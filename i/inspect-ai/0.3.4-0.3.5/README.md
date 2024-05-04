# Comparing `tmp/inspect_ai-0.3.4.tar.gz` & `tmp/inspect_ai-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspect_ai-0.3.4.tar", last modified: Wed May  1 18:12:02 2024, max compression
+gzip compressed data, was "inspect_ai-0.3.5.tar", last modified: Sat May  4 21:23:47 2024, max compression
```

## Comparing `inspect_ai-0.3.4.tar` & `inspect_ai-0.3.5.tar`

### file list

```diff
@@ -1,368 +1,369 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.028439 inspect_ai-0.3.4/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/arc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.028439 inspect_ai-0.3.4/benchmarks/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/datasets/math_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/datasets/mmlu.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/gpqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/gsm8k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/hellaswag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/mathematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/mmlu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.028439 inspect_ai-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.032439 inspect_ai-0.3.4/docs/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/arc.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/biology_qa.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/footer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/gsm8k.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/hellaswag.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/mathematics.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/popularity.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/security_guide.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/theory_of_mind.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/tool_use.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.032439 inspect_ai-0.3.4/docs/_format/
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_format/pre-render.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_variables.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/datasets.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/eval-logs.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/eval-suites.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/eval-tuning.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/examples.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/aisi-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/eval-log.png
--rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-answers.png
--rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-history.png
--rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-home.png
--rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-info.png
--rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-logging-console.png
--rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-logging.png
--rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-main.png
--rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-messages.png
--rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-metadata.png
--rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-scoring.png
--rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-sort.png
--rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/popularity.png
--rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/rate-limit.png
--rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/running-theory.png
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/log-viewer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/models.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/scorers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/solvers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/theme.scss
--rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/tools.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    12352 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/workflow.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.020439 inspect_ai-0.3.4/examples/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/examples/agents/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/.env.example
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/inspect_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/wikipedia.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/biology_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/popularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/security_guide.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/theory_of_mind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/tool_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.020439 inspect_ai-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/src/inspect_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.044439 inspect_ai-0.3.4/src/inspect_ai/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/score.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.044439 inspect_ai-0.3.4/src/inspect_ai/_display/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/rich.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.044439 inspect_ai-0.3.4/src/inspect_ai/_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/score.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.048439 inspect_ai-0.3.4/src/inspect_ai/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.048439 inspect_ai-0.3.4/src/inspect_ai/_view/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.048439 inspect_ai-0.3.4/src/inspect_ai/_view/www/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/App.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/api.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.020439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/json5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/purify.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/showdown.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/log-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/log.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/hooks.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/htm.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/preact.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/preact.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/preact-hooks.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/preact.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/Constants.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/Register.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Card.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ChatView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/CopyButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Dialog.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MessageContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/TabSet.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ToolButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ansi-output.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/title/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Format.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Git.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Path.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Type.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/tools.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/bias_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/biology_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/popularity.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/security_guide.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.064438 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.064438 inspect_ai-0.3.4/src/inspect_ai/log/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/log/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.064438 inspect_ai-0.3.4/src/inspect_ai/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31676 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/model/_providers/
--rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/azureai.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/together.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/scorer/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_critique.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_multiple_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.072439 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/use_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.072439 inspect_ai-0.3.4/src/inspect_ai/util/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.072439 inspect_ai-0.3.4/src/inspect_ai/util/_context/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/src/inspect_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-05-01 18:12:02.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_cloudlfare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_collapse_user_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset/samples.csv
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset/samples.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset/samples.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_eval_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_images/
--rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_images/images.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_list_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_logprobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_num_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_stop_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/attribs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/_decoy/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/_decoy/testit.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/_decoy2.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/tests/test_task_list/recurse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/recurse/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/.folder3/epsilon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/recurse/folder1/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder1/_decoy.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder1/theta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/another.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/first.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.347093 inspect_ai-0.3.5/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/arc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.347093 inspect_ai-0.3.5/benchmarks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/datasets/math_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/datasets/mmlu.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/gpqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/gsm8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/hellaswag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/mathematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/mmlu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.351093 inspect_ai-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.351093 inspect_ai-0.3.5/docs/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/arc.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/biology_qa.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/footer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/gsm8k.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/hellaswag.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/mathematics.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/popularity.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/security_guide.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/theory_of_mind.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/tool_use.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.351093 inspect_ai-0.3.5/docs/_format/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_format/pre-render.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_variables.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/datasets.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/eval-logs.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/eval-suites.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/eval-tuning.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/examples.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.359093 inspect_ai-0.3.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/aisi-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/eval-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-answers.png
+-rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-info.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-logging-console.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-logging.png
+-rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-main.png
+-rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-messages.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-scoring.png
+-rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-sort.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/popularity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/rate-limit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/running-theory.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/log-viewer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/models.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/scorers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/solvers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/tools.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/workflow.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.359093 inspect_ai-0.3.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.335093 inspect_ai-0.3.5/examples/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.363093 inspect_ai-0.3.5/examples/agents/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/inspect_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/wikipedia.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/biology_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/security_guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/theory_of_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/tool_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.335093 inspect_ai-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.363093 inspect_ai-0.3.5/src/inspect_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.367093 inspect_ai-0.3.5/src/inspect_ai/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.367093 inspect_ai-0.3.5/src/inspect_ai/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/rich.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.367093 inspect_ai-0.3.5/src/inspect_ai/_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.371093 inspect_ai-0.3.5/src/inspect_ai/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.371093 inspect_ai-0.3.5/src/inspect_ai/_view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/App.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/api.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.339093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/json5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/showdown.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/log-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/log.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.379094 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/hooks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.379094 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/htm.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/preact.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/preact.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/preact-hooks.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/preact.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.379094 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/Constants.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/Register.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Card.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ChatView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/CopyButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Dialog.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MessageContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/TabSet.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ToolButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ansi-output.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/title/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Format.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Git.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Path.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Type.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/tools.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/bias_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/biology_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/popularity.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/security_guide.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/log/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.391093 inspect_ai-0.3.5/src/inspect_ai/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31683 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.391093 inspect_ai-0.3.5/src/inspect_ai/model/_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/azureai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.391093 inspect_ai-0.3.5/src/inspect_ai/scorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/use_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/util/_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/src/inspect_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.399093 inspect_ai-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_cloudlfare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_collapse_user_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset/samples.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset/samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset/samples.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_eval_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_images/images.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_list_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_logprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_num_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_stop_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/attribs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/_decoy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/_decoy/testit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/_decoy2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/tests/test_task_list/recurse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/.folder3/epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/folder1/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder1/_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder1/theta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/utils.py
```

### Comparing `inspect_ai-0.3.4/.github/workflows/build.yml` & `inspect_ai-0.3.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/.github/workflows/docs.yml` & `inspect_ai-0.3.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/.github/workflows/pypi.yml` & `inspect_ai-0.3.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/.gitignore` & `inspect_ai-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/.pre-commit-config.yaml` & `inspect_ai-0.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/CHANGELOG.md` & `inspect_ai-0.3.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## v0.3.5 (04 May 2024)
+
+- Fix issue with logs from S3 buckets in inspect view.
+- Add `sort()` method to `Dataset` (defaults to sorting by sample input length).
+- Improve tokenization for HF provider (left padding, attention mask, and allow for custom chat template)
+- Improve batching for HF provider (generate as soon as queue fills, thread safety for future.set_result).
+- Various improvements to documentation.
+
 ## v0.3.4 (01 May 2024)
 
 - `write_eval_log()` now ignores unserializable objects in metadata fields.
 - `read_eval_log()` now takes a `str` or `FileInfo` (for compatibility w/ list returned from `list_eval_logs()`).
 - Registry name looks are now case sensitive (fixes issue w/ loading tasks w/ mixed case names).
 - Resiliancy to Python syntax errors that occur when enumerating tasks in a directory.
 - Do not throw error if unable to parse or load `.ipynb` file due to lack of dependencies (e.g. `nbformat`).
```

### Comparing `inspect_ai-0.3.4/LICENSE` & `inspect_ai-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/PKG-INFO` & `inspect_ai-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.4
+Version: 0.3.5
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
@@ -60,14 +60,15 @@
 Requires-Dist: openai; extra == "dev"
 Requires-Dist: anthropic; extra == "dev"
 Requires-Dist: google-cloud-aiplatform; extra == "dev"
 Requires-Dist: google-generativeai; extra == "dev"
 Requires-Dist: mistralai; extra == "dev"
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: transformers; extra == "dev"
+Requires-Dist: accelerate; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: datasets; extra == "dev"
 Requires-Dist: langchain; extra == "dev"
 Requires-Dist: langchainhub; extra == "dev"
 Requires-Dist: wikipedia; extra == "dev"
 Requires-Dist: ipywidgets; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
```

### Comparing `inspect_ai-0.3.4/README.md` & `inspect_ai-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/benchmarks/README.md` & `inspect_ai-0.3.5/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/benchmarks/arc.py` & `inspect_ai-0.3.5/benchmarks/arc.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/benchmarks/gpqa.py` & `inspect_ai-0.3.5/benchmarks/gpqa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/benchmarks/gsm8k.py` & `inspect_ai-0.3.5/benchmarks/gsm8k.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/benchmarks/hellaswag.py` & `inspect_ai-0.3.5/benchmarks/hellaswag.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/benchmarks/mathematics.py` & `inspect_ai-0.3.5/benchmarks/mathematics.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/benchmarks/mmlu.py` & `inspect_ai-0.3.5/benchmarks/mmlu.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/arc.qmd` & `inspect_ai-0.3.5/docs/_examples/arc.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/biology_qa.qmd` & `inspect_ai-0.3.5/docs/_examples/biology_qa.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/footer.qmd` & `inspect_ai-0.3.5/docs/_examples/footer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/gsm8k.qmd` & `inspect_ai-0.3.5/docs/_examples/gsm8k.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/hellaswag.qmd` & `inspect_ai-0.3.5/docs/_examples/hellaswag.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/index.qmd` & `inspect_ai-0.3.5/docs/_examples/index.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/mathematics.qmd` & `inspect_ai-0.3.5/docs/_examples/mathematics.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/popularity.qmd` & `inspect_ai-0.3.5/docs/_examples/popularity.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/security_guide.qmd` & `inspect_ai-0.3.5/docs/_examples/security_guide.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/theory_of_mind.qmd` & `inspect_ai-0.3.5/docs/_examples/theory_of_mind.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_examples/tool_use.qmd` & `inspect_ai-0.3.5/docs/_examples/tool_use.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/_quarto.yml` & `inspect_ai-0.3.5/docs/_quarto.yml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    downloads: [pdf, epub, docx]
    twitter-card:
       description: "Open-source framework for large language model evaluations"
    open-graph: 
       description: "Open-source framework for large language model evaluations"
    sidebar:
       header: >
-         [![](images/aisi-logo.png)](https://www.gov.uk/government/organisations/ai-safety-institute)
+         [![](images/aisi-logo.png){fig-alt="UK AI Safety Institute Website"}](https://www.gov.uk/government/organisations/ai-safety-institute)
 
    page-footer: 
       left: 
          - text: UK AI Safety Institute
            href: https://www.gov.uk/government/organisations/ai-safety-institute
       center: 
          - text: Code
```

### Comparing `inspect_ai-0.3.4/docs/datasets.qmd` & `inspect_ai-0.3.5/docs/datasets.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/eval-logs.qmd` & `inspect_ai-0.3.5/docs/eval-logs.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 Every time you use `inspect eval` or call the `eval()` function, an evaluation log is written for each task evaluated. By default, logs are written to the `./logs` sub-directory of the current working directory (we'll cover how to change this below). You will find a link to the log at the bottom of the results for each task:
 
 ``` bash
 $ inspect eval security_guide.py --model openai/gpt-4
 ```
 
-![](images/eval-log.png)
+![](images/eval-log.png){fig-alt="The Inspect task results displayed in the terminal. A link to the evaluation log is at the bottom of the results display."}
 
 You can also use the Inspect log viewer for interactive exploration of logs. Run this command once at the beginning of a working session (the view will update automatically when new evaluations are run):
 
 ```bash
 $ inspect view
 ```
 
-![](images/inspect-view-main.png){.border .lightbox}
+![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 8 individual samples."}
 
 This section won't cover using `inspect view` though. Rather, it will cover the details of managing log usage from the CLI as well as the Python API for reading logs. See the [Log Viewer](#sec-log-viewer)  section for details on interactively exploring logs.
 
 
 ## Log Location
 
 By default, logs are written to the `./logs` sub-directory of the current working directory You can change where logs are written using eval options or an environment variable
```

### Comparing `inspect_ai-0.3.4/docs/eval-suites.qmd` & `inspect_ai-0.3.5/docs/eval-suites.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/eval-tuning.qmd` & `inspect_ai-0.3.5/docs/eval-tuning.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 The default value for max connections is 10. By increasing it we might get better performance due to higher parallelism, however we might get _worse_ performance if this causes us to frequently hit rate limits (which are retried with exponential backoff). The "correct" max connections for your evaluations will vary based on your actual rate limit and the size and complexity of your evaluations. 
 
 
 ### Rate Limits 
 
 When you run an eval you'll see information reported on the current active connection usage as well as the number of HTTP rate limit errors that have been encountered (note that Inspect will automatically retry on rate limits and other errors likely to be transient):
 
-![](images/rate-limit.png)
+![](images/rate-limit.png){fig-alt="The Inspect task results displayed in the terminal. The number of HTTP rate limit errors that have occurred (25) is printed in the bottom right of the task results."}
 
 Here we've set a higher max connections than the default (30). While you might be tempted to set this very high to see how much concurrent traffic you can sustain, more often than not setting too high a max connections will result in slower evaluations, because retries are done using [exponential backoff](https://en.wikipedia.org/wiki/Exponential_backoff), and bouncing off of rate limits too frequently will have you waiting minutes for retries to fire.
 
 You should experiment with various values for max connections at different times of day (evening is often very different than daytime!). Generally speaking, you want to see some number of HTTP rate limits enforced so you know that are somewhere close to ideal utilisation, but if you see hundreds of these you are likely over-saturating and experiencing a net slowdown.
 
 ### Limiting Retries
```

### Comparing `inspect_ai-0.3.4/docs/examples.qmd` & `inspect_ai-0.3.5/docs/examples.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/aisi-logo.png` & `inspect_ai-0.3.5/docs/images/aisi-logo.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/eval-log.png` & `inspect_ai-0.3.5/docs/images/eval-log.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-answers.png` & `inspect_ai-0.3.5/docs/images/inspect-view-answers.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-filter.png` & `inspect_ai-0.3.5/docs/images/inspect-view-filter.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-history.png` & `inspect_ai-0.3.5/docs/images/inspect-view-history.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-home.png` & `inspect_ai-0.3.5/docs/images/inspect-view-home.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-info.png` & `inspect_ai-0.3.5/docs/images/inspect-view-info.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-logging-console.png` & `inspect_ai-0.3.5/docs/images/inspect-view-logging-console.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-logging.png` & `inspect_ai-0.3.5/docs/images/inspect-view-logging.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-main.png` & `inspect_ai-0.3.5/docs/images/inspect-view-main.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-messages.png` & `inspect_ai-0.3.5/docs/images/inspect-view-messages.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-metadata.png` & `inspect_ai-0.3.5/docs/images/inspect-view-metadata.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-scoring.png` & `inspect_ai-0.3.5/docs/images/inspect-view-scoring.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-sort.png` & `inspect_ai-0.3.5/docs/images/inspect-view-sort.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/inspect-view-splash.png` & `inspect_ai-0.3.5/docs/images/inspect-view-splash.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/popularity.png` & `inspect_ai-0.3.5/docs/images/popularity.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/rate-limit.png` & `inspect_ai-0.3.5/docs/images/rate-limit.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/images/running-theory.png` & `inspect_ai-0.3.5/docs/images/running-theory.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/index.qmd` & `inspect_ai-0.3.5/docs/index.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 - Scale up to more sophsisticated evals with multi-turn dialog, agent scaffolds and model grading.
 
 - Interactive workflows for researchers; production workflows for larger evaluation suites. 
 
 - Adapt and extend the framework with custom Python components.
 
-![](images/inspect-view-splash.png){.lightbox .border}
+![](images/inspect-view-splash.png){.lightbox .border fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 5 individual samples."}
 
 :::
 
 ## Welcome
 
 Welcome to Inspect, a framework for large language model evaluations created by the [UK AI Safety Institute](https://www.gov.uk/government/organisations/ai-safety-institute).
 
@@ -138,25 +138,25 @@
 
 The `@task` decorator applied to the `theory_of_mind()` function is what enables `inspect eval` to find and run the eval in the source file passed to it. For example, here we run the eval against GPT-4:
 
 ``` bash
 $ inspect eval theory_of_mind.py --model openai/gpt-4
 ```
 
-![](images/running-theory.png)
+![](images/running-theory.png){fig-alt="The Inspect task results displayed in the terminal. A progress bar indicates that the evaluation is about 60% complete."}
 
 By default, eval logs are written to the `./logs` sub-directory of the current working directory. When the eval is complete you will find a link to the log at the bottom of the task results summary.
 
 You can also explore eval results using the Inspect log viewer. Run `inspect view` to open the viewer (you only need to do this once as the viewer will automatically updated when new evals are run):
 
 ```bash
 $ inspect view
 ```
 
-![](images/inspect-view-home.png){.border .lightbox}
+![](images/inspect-view-home.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 7 individual samples."}
 
 See the [Log Viewer](#sec-log-viewer) section for additional details on using Inspect View.
 
 ::: {.callout-note appearance="simple"}
 This example demonstrates evals being run from the terminal with the `inspect eval` command. There is also an `eval()` function which can be used for exploratory work---this is covered further in [Workflow](#sec-workflow).
 :::
```

### Comparing `inspect_ai-0.3.4/docs/log-viewer.qmd` & `inspect_ai-0.3.5/docs/log-viewer.qmd`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Log Viewer {#sec-log-viewer}
 
 ## Overview
 
 Inspect View provides a convenient way to visualise evaluation logs, including drilling into message histories, scoring decisions, and additional metadata written to the log. Here's what the main view of an evaluation log looks like:
 
-![](images/inspect-view-main.png){.border .lightbox}
+![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 8 individual samples."}
 
 Below we'll describe how to get the most out of using Inspect View.
 
 Note that this section covers *interactively* exploring log files. You can also use the `EvalLog` API to compute on log files (e.g. to compare across runs or to more systematically traverse results). See the section on [Eval Logs](#sec-eval-logs) to learn more about how to process log files with code.
 
 ## View Basics
 
@@ -32,54 +32,54 @@
 
 You only need to run `inspect view` once at the beginning of a session (as it will automatically update to show new evaluations when they are run).
 
 ### Log History
 
 You can view and navigate between a history of all evals in the log directory using the menu at the top right:
 
-![](images/inspect-view-history.png){.border .lightbox}
+![](images/inspect-view-history.png){.border .lightbox fig-alt="The Inspect log viewer, with the history panel displayed on the left overlaying the main interface. Several log files are displayed in the log history, each of which includes a summary of the results."}
 
 ## Sample Details
 
 Click a sample to drill into its messages, scoring, and metadata.
 
 ### Messages
 
 The messages tab displays the message history. In this example we see that the model make two tool calls before answering (the final assistant message is not fully displayed for brevity):
 
-![](images/inspect-view-messages.png){.border .lightbox}
+![](images/inspect-view-messages.png){.border .lightbox fig-alt="The Inspect log viewer showing a sample expanded, with details on the user, assistant, and tool messages for the sample."}
 
 Looking carefully at the message history (especially for agents or multi-turn solvers) is critically important for understanding how well your evaluation is constructed.
 
 ### Scoring
 
 The scoring tab shows additional details including the full input and full model explanation for answers:
 
-![](images/inspect-view-scoring.png){.border .lightbox}
+![](images/inspect-view-scoring.png){.border .lightbox fig-alt="The Inspect log viewer showing a sample expanded, with details on the scoring of the sample, including the input, target, answer, and explanation."}
 
 ### Metadata
 
 The metadata tab shows additional data made available by solvers, tools, an scorers (in this case the `web_search()` tool records which URLs it visited to retreive additional context):
 
-![](images/inspect-view-metadata.png){.border .lightbox}
+![](images/inspect-view-metadata.png){.border .lightbox fig-alt="The Inspect log viewer showing a sample expanded, with details on the metadata recorded by the web search tool during the evaluation (specifically, the URLs queried by the web search tool for the sample)."}
 
 ## Scores and Answers
 
 Reliable, high quality scoring is a critical component of every evaluation, and developing custom scorers that deliver this can be challenging. One major difficulty lies in the free form text nature of model output: we have a very specific target we are comparing against and we sometimes need to pick the answer out of a sea of text. Model graded output introduces another set of challenges entirely.
 
 For comparison based scoring, scorers typically perform two core tasks:
 
 1.  Extract the answer from the model's output; and
 2.  Compare the extracted answer to the target.
 
 A scorer can fail to correctly score output at either of these steps. Failing to extract an answer entirely can occur (e.g. due to a regex that's not quite flexible enough) and as can failing to correctly identify equivalent answers (e.g. thinking that "1,242" is different from "1242.00" or that "Yes." is different than "yes").
 
 You can use the log viewer to catch and evaluate these sorts of issues. For example, here we can see that we were unable to extract answers for a couple of questions that were scored incorrect:
 
-![](images/inspect-view-answers.png){.border .lightbox}
+![](images/inspect-view-answers.png){.border .lightbox fig-alt="The Inspect log viewer with several 5 samples displayed, 3 of which are incorrect. The Answer column displays the answer extracted from the model output for each sample."}
 
 It's possible that these answers are legitimately incorrect. However it's also possible that the correct answer is in the model's output but just in a format we didn't quite expect. In each case you'll need to drill into the sample to investigate.
 
 Answers don't just appear magically, scorers need to produce them during scoring. The scorers built in to Inspect all do this, but when you create a custom scorer, you should be sure to always include an `answer` in the `Score` objects you return if you can. For example:
 
 ``` python
 return Score(
@@ -93,19 +93,19 @@
 
 Note there is also an `explanation` field: this is also important, as it allows you to view the entire context from which the answer was extracted from.
 
 ## Filtering and Sorting
 
 It's often useful to filter log entries by score (for example, to investigate whether incorrect answers are due to scorer issues or are true negatives). Use the **Scores** picker to filter by specific scores:
 
-![](images/inspect-view-filter.png){.border .lightbox}
+![](images/inspect-view-filter.png){.border .lightbox fig-alt="The Inspect log view, with 4 samples displayed, each of which are marked incorrect. The Scores picker is focused, and has selected 'Incorrect', indicating that only incorrect scores should be displayed."}
 
 By default, samples are ordered (with all samples for an epoch presented in sequence). However you can also order by score, or order by samples (so you see all of the results for a given sample across all epochs presented together). Use the **Sort** picker to control this:
 
-![](images/inspect-view-sort.png){.border .lightbox}
+![](images/inspect-view-sort.png){.border .lightbox fig-alt="The Inspect log view, with the results of a single sample for each of the 4 epochs of the evaluation."}
 
 Viewing by sample can be especially valuable for diagnosing the sources of inconsistency (and determining whether they are inherent or an artifact of the evaluation methodology). Above we can see that sample 1 is incorrect in epoch 1 because of issue the model had with forming a correct function call.
 
 ## Python Logging
 
 Beyond the standard information included an eval log file, you may want to do additional console logging to assist with developing and debugging. Inspect installs a log handler that displays logging output above eval progress as well as saves it into the evaluation log file.
 
@@ -117,26 +117,26 @@
 
 # log each time we see a web query
 logger.info(f"web query: {query}")
 ```
 
 You can see all of these log entries in the **Logging** tab:
 
-![](images/inspect-view-logging.png){.border .lightbox}
+![](images/inspect-view-logging.png){.border .lightbox fig-alt="The Logging panel of the Inspect log viewer, displaying several info log messages from the web search tool indicating what queries were executed by the tool."}
 
 It is important to note that the Inspect View will show all log entries level `info` or higher. However, printing every `info` message to the console during an eval might be too distracting, so the default log level for printing is `warning`. If you change it to `info` then you'll also see these log messages in the console:
 
 ``` bash
 $ inspect eval biology_qa.py --log-level info
 ```
 
-![](images/inspect-view-logging-console.png){.lightbox}
+![](images/inspect-view-logging-console.png){.lightbox fig-alt="This Inspect task display in the terminal, with several info log messages from the web search tool printed above the the task diplay."}
 
 A default log level of `warning` enables you to include many calls to `logger.info()` in your code without having them show by default, while also making them available in the log viewer should you need them.
 
 Note that you can also set the log level using the `INSPECT_LOG_LEVEL` environment variable (which is often included in a [.env configuration file](#sec-workflow-configuration)).
 
 ## Task Information
 
 The **Info** panel of the log viewer provides additional meta-information about evaluation tasks, including dataset, plan, and scorer details, git revision, and model token usage:
 
-![](images/inspect-view-info.png){style=".border .lightbox"}
+![](images/inspect-view-info.png){.border .lightbox fig-alt="The Info panel of the Inspect log viewer, displaying various details about the evaluation including dataset, plan, and scorer details, git revision, and model token usage."}
```

### Comparing `inspect_ai-0.3.4/docs/models.qmd` & `inspect_ai-0.3.5/docs/models.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
      ],
      scorer=model_graded_fact(model = grader_model),
   )
 ```
 
 ## Model Args
 
-The section above illustrates passing model specific arguments to local models on the command line, in `eval()`, and in `get_model()`. This actually works for all model types, so if there is an additional aspect of a modal you want to tweak that isn't covered by the `GenerationConfig`, you can use this method to do it. For example, here we specify the `transport` option for a Google Gemini model:
+The section above illustrates passing model specific arguments to local models on the command line, in `eval()`, and in `get_model()`. This actually works for all model types, so if there is an additional aspect of a model you want to tweak that isn't covered by the `GenerationConfig`, you can use this method to do it. For example, here we specify the `transport` option for a Google Gemini model:
 
 ``` bash
 inspect eval popularity --model google/gemini-1.0-pro -M transport:grpc
 ```
 
 The additional `model_args` are forwarded as follows for the various providers:
 
@@ -354,8 +354,8 @@
 # get a model instance
 model = get_model("custom/name-of-model")
 
 # run an eval with the model
 eval(math, model = "custom/name-of-model")
 ```
 
-In this example, the `model_name` argument passed to `__init__()` will be "name-of-model".
+In this example, the `model_name` argument passed to `__init__()` will be "name-of-model".
```

### Comparing `inspect_ai-0.3.4/docs/scorers.qmd` & `inspect_ai-0.3.5/docs/scorers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/solvers.qmd` & `inspect_ai-0.3.5/docs/solvers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/docs/theme.scss` & `inspect_ai-0.3.5/docs/theme.scss`

 * *Files 13% similar despite different names*

```diff
@@ -42,7 +42,10 @@
 
 @media(max-width: 991.98px) {
     .sidebar-header-item .img-fluid {
         max-width: 195px;
     }
 }
 
+.blockquote {
+    color: #505a62;
+}
```

### Comparing `inspect_ai-0.3.4/docs/tools.qmd` & `inspect_ai-0.3.5/docs/tools.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
 -   `max_provider_calls`---Number of times to retrieve more links from the search provider incase previous ones were irrelevant (defaults to 3)
 
 -   `max_connections`---Maximum number of concurrent connections to the search API provider (defaults to 10).
 
 -   `model`---Model to use to determine if search results are relevant (defaults to the model currently being evaluated).
 
-#### Google Provider
+### Google Provider
 
 The `web_search()` tool uses [Google Programmable Search Engine](https://programmablesearchengine.google.com/about/). To use it you will therefore need to setup your own Google Programmable Search Engine and also enable the [Programmable Search Element Paid API](https://developers.google.com/custom-search/docs/paid_element). Then, ensure that the following environment variables are defined:
 
 -   `GOOGLE_CSE_ID` — Google Custom Search Engine ID
 
 -   `GOOGLE_CSE_API_KEY` — Google API key used to enable the Search API
```

### Comparing `inspect_ai-0.3.4/docs/workflow.qmd` & `inspect_ai-0.3.5/docs/workflow.qmd`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 You can run this evaluation from the shell using the `inspect eval` command. For example:
 
 ``` bash
 $ inspect eval theory.py --model openai/gpt-4
 ```
 
-![](images/running-theory.png)
+![](images/running-theory.png){fig-alt="The Inspect task results displayed in the terminal. A progress bar indicates that the evaluation is about 60% complete."}
 
 Immediately after an evaluation completes, a link to the log for the evaluation is written to the terminal (if you are running in VS Code this link will open the log in an editor within the IDE).
 
 ### Models
 
 Run the evaluation against other models as follows:
 
@@ -63,20 +63,20 @@
 
 As you iterate on an evaluation, you'll typically want to dig further into message histories, scoring decisions, and other diagnostics. Typically at the outset of working session you'll run `inspect view` to open the Inspect [Log Viewer](#sec-log-viewer):
 
 ``` bash
 $ inspect view
 ```
 
-![](images/inspect-view-main.png){.border .lightbox}
+![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 8 individual samples."}
 
 
 The log viewer will update automatically whenever a new evaluation is completed (you can also navigate back to previous evaluations). The log viewer summarises aggregate data and also provides a detailed view into each sample. For example, here we zoom in on the model's scoring explanation for a specific sample:
 
-![](images/inspect-view-scoring.png){.border .lightbox}
+![](images/inspect-view-scoring.png){.border .lightbox fig-alt="The Inspect log viewer showing a sample expanded, with details on the scoring of the sample, including the input, target, answer, and explanation."}
 
 See the [Log Viewer](#sec-log-viewer) section for additional details on using Inspect View.
 
 ### Options
 
 There are several other command line options you can pass to eval. Here are some of the more useful ones:
```

### Comparing `inspect_ai-0.3.4/examples/agents/langchain/README.md` & `inspect_ai-0.3.5/examples/agents/langchain/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/agents/langchain/inspect_langchain.py` & `inspect_ai-0.3.5/examples/agents/langchain/inspect_langchain.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/agents/langchain/wikipedia.jsonl` & `inspect_ai-0.3.5/examples/agents/langchain/wikipedia.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/agents/langchain/wikipedia.py` & `inspect_ai-0.3.5/examples/agents/langchain/wikipedia.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/biology_qa.py` & `inspect_ai-0.3.5/examples/biology_qa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/popularity.py` & `inspect_ai-0.3.5/examples/popularity.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/security_guide.py` & `inspect_ai-0.3.5/examples/security_guide.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/theory_of_mind.py` & `inspect_ai-0.3.5/examples/theory_of_mind.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/examples/tool_use.py` & `inspect_ai-0.3.5/examples/tool_use.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/pyproject.toml` & `inspect_ai-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     "openai",
     "anthropic",
     "google-cloud-aiplatform",
     "google-generativeai",
     "mistralai",
     "boto3",
     "transformers",
+    "accelerate",
     "torch",
     "datasets",
     "langchain",
     "langchainhub",
     "wikipedia",
     "ipywidgets",
     "ipython",
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai/__init__.py` & `inspect_ai-0.3.5/src/inspect_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/common.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/eval.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/eval.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/info.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/info.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/list.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/list.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/main.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/main.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/score.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/util.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_cli/view.py` & `inspect_ai-0.3.5/src/inspect_ai/_cli/view.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_display/_display.py` & `inspect_ai-0.3.5/src/inspect_ai/_display/_display.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_display/logger.py` & `inspect_ai-0.3.5/src/inspect_ai/_display/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_display/rich.py` & `inspect_ai-0.3.5/src/inspect_ai/_display/rich.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/eval.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/eval.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/images.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/list.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/list.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/loader.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/loader.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/log.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/registry.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/score.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_eval/task.py` & `inspect_ai-0.3.5/src/inspect_ai/_eval/task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/dotenv.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/dotenv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/error.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/error.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/file.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/git.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/git.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/http.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/http.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/images.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/json.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/notebook.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/notebook.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/path.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/path.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/platform.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/platform.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/registry.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/retry.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_util/url.py` & `inspect_ai-0.3.5/src/inspect_ai/_util/url.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/schema.py` & `inspect_ai-0.3.5/src/inspect_ai/_view/schema.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/view.py` & `inspect_ai-0.3.5/src/inspect_ai/_view/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from functools import partial
 from http import HTTPStatus
 from http.server import HTTPServer
 from io import BytesIO
 from pathlib import Path
 from typing import Any
-from urllib.parse import parse_qs, urlparse
+from urllib.parse import parse_qs, urlparse, urlunparse
 
 import psutil
 
 from inspect_ai._display import display
 from inspect_ai._display.logger import init_logger
 from inspect_ai._util.appdirs import inspect_runtime_dir
 from inspect_ai._util.constants import (
@@ -124,18 +124,31 @@
     def handle_log(self) -> None:
         """Serve log files from /api/logs/* url."""
         path = self.path.replace(LOGS_DIR, "", 1)  # strip /api/logs/
         path = path.replace("..", "")  # no escape
 
         # check for query params
         parsed = urlparse(path)
-        path = parsed.path
+
+        # read query parameters from the URL
         query_params = parse_qs(parsed.query)
         header_only = query_params.get("header-only", None) is not None
 
+        # reconstruct the path
+        path = urlunparse(
+            (
+                parsed.scheme,
+                parsed.netloc,
+                parsed.path,
+                parsed.params,
+                "",  # Clear the query component
+                parsed.fragment,
+            )
+        )
+
         ctype = self.guess_type(path)
         try:
             contents: bytes | None = None
             if header_only:
                 try:
                     log = read_eval_log(path, header_only=True)
                     contents = eval_log_json(log).encode()
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/App.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/App.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/api.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/api.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/favicon.svg` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/favicon.svg`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/index.html` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/index.html`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/clipboard.min.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/json5.min.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/json5.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism-dark.css` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism-dark.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.css` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/purify.min.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/purify.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/showdown.min.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/showdown.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/log-schema.json` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/log-schema.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/log.d.ts` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/log.d.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/hooks.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/hooks.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/htm.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/htm.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/preact.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/preact.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/App.css` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/App.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/Constants.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/Constants.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.css` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Card.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Card.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ChatView.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ChatView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/CopyButton.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/CopyButton.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Dialog.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Dialog.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LabeledValue.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LabeledValue.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MessageContent.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MessageContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MetaDataView.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MetaDataView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/RenderedContent.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/RenderedContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/TabSet.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/TabSet.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ansi-output.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ansi-output.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/plan/PlanCard.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/plan/PlanCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleView.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/title/TitleBlock.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/title/TitleBlock.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/UsageCard.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/UsageCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Format.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Format.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/_view/www/tools.js` & `inspect_ai-0.3.5/src/inspect_ai/_view/www/tools.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/__init__.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_dataset.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 import abc
 import random
-from typing import Any, Callable, Iterator, Sequence, Union, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterator,
+    Optional,
+    Sequence,
+    Union,
+    overload,
+)
 
 from pydantic import BaseModel, Field
 from typing_extensions import override
 
 from inspect_ai.model import ChatMessage
 
+if TYPE_CHECKING:
+    from _typeshed import SupportsRichComparison
+
 
 class Sample(BaseModel):
     r"""Sample to be used in an evaluation task.
 
     Args:
         input (str | list[ChatMessage]): The input to be submitted to the model.
         choices (list[str] | None): Optional. List of available answer choices
@@ -33,75 +45,97 @@
     id: int | str | None = Field(default=None)
     """Unique identifier for sample."""
 
     metadata: dict[str, Any] | None = Field(default=None)
     """Arbitrary metadata associated with the sample."""
 
 
+def sample_input_len(sample: Sample) -> int:
+    """Measures the length of a samples `input` field.
+
+    The default length function use in `Dataset.sort()`.
+
+    Args:
+        sample (Sample): A Sample to be used in an evaluation task.
+    """
+    return (
+        len(sample.input)
+        if isinstance(sample.input, str)
+        else sum(len(inp.text) for inp in sample.input)
+    )
+
+
 DatasetRecord = dict[str, Any]
 
 DatasetReader = Iterator[DatasetRecord]
 
 
 class Dataset(Sequence[Sample], abc.ABC):
     r"""A sequence of Sample objects.
 
     Datasets provide sequential access (via conventional indexes or slicing)
     to a collection of Sample objects.
     """
 
     @abc.abstractproperty
-    def name(self) -> str | None:
-        ...
+    def name(self) -> str | None: ...
 
     @abc.abstractproperty
-    def location(self) -> str | None:
-        ...
+    def location(self) -> str | None: ...
 
     @overload
-    def __getitem__(self, index: int) -> Sample:
-        ...
+    def __getitem__(self, index: int) -> Sample: ...
 
     @overload
-    def __getitem__(self, index: slice) -> "Dataset":
-        ...
+    def __getitem__(self, index: slice) -> "Dataset": ...
 
     @abc.abstractmethod
-    def __getitem__(self, index: Union[int, slice]) -> Union[Sample, "Dataset"]:
-        ...
+    def __getitem__(self, index: Union[int, slice]) -> Union[Sample, "Dataset"]: ...
 
     @abc.abstractmethod
-    def __len__(self) -> int:
-        ...
+    def __len__(self) -> int: ...
 
     @abc.abstractmethod
     def shuffle(self, seed: int | None = None) -> None:
         """Shuffle the order of the dataset (in place).
 
         Args:
            seed: (int | None): Random seed for shuffling (optional).
         """
 
+    @abc.abstractmethod
+    def sort(
+        self,
+        reverse: bool = False,
+        key: Optional[Callable[[Sample], "SupportsRichComparison"]] = sample_input_len,
+    ) -> None:
+        """Sort the dataset (in place) in ascending order and return None.
+
+        If a key function is given, apply it once to each list item and sort them, ascending or descending, according to their function values.
+
+        The key function defaults to measuring the length of the sample's input field.
+
+        Args:
+            reverse (bool): if true, sort in descending order. Defaults to False.
+            key (Callable[[Any], Any]): a callable mapping each item to a numeric value (optional, defaults to sample_input_len).
+        """
+
+    @abc.abstractmethod
     def filter(
         self, predicate: Callable[[Sample], bool], name: str | None = None
     ) -> "Dataset":
         """Filter the dataset using a predicate.
 
         Args:
           predicate (Callable[[Sample], bool]): Filtering function.
           name (str | None): Name for filtered dataset (optional).
 
         Returns:
           Filtered dataset.
         """
-        return MemoryDataset(
-            name=name or self.name,
-            location=self.location,
-            samples=[sample for sample in self if predicate(sample)],
-        )
 
 
 class FieldSpec(BaseModel):
     r"""Specification for mapping data source fields to sample fields.
 
     Args:
         input (str): Name of the field containing the sample input.
@@ -164,20 +198,18 @@
     @override
     @property
     def location(self) -> str | None:
         """Dataset location."""
         return self._location
 
     @overload
-    def __getitem__(self, index: int) -> Sample:
-        ...
+    def __getitem__(self, index: int) -> Sample: ...
 
     @overload
-    def __getitem__(self, index: slice) -> Dataset:
-        ...
+    def __getitem__(self, index: slice) -> Dataset: ...
 
     @override
     def __getitem__(self, index: Union[int, slice]) -> Union[Sample, Dataset]:
         if isinstance(index, int):
             return self.samples[index]
         else:
             return MemoryDataset(
@@ -190,7 +222,25 @@
 
     @override
     def shuffle(self, seed: int | None = None) -> None:
         if seed:
             random.Random(seed).shuffle(self.samples)
         else:
             random.shuffle(self.samples)
+
+    @override
+    def sort(
+        self,
+        reverse: bool = False,
+        key: Optional[Callable[[Sample], "SupportsRichComparison"]] = sample_input_len,
+    ) -> None:
+        self.samples.sort(reverse=reverse, key=key)
+
+    @override
+    def filter(
+        self, predicate: Callable[[Sample], bool], name: str | None = None
+    ) -> "MemoryDataset":
+        return MemoryDataset(
+            name=name or self.name,
+            location=self.location,
+            samples=[sample for sample in self if predicate(sample)],
+        )
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/bias_detection.jsonl` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/bias_detection.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/biology_qa.jsonl` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/biology_qa.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/popularity.jsonl` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/popularity.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/security_guide.jsonl` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/security_guide.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/csv.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/csv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/example.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/example.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/file.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/hf.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/json.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/dataset/_util.py` & `inspect_ai-0.3.5/src/inspect_ai/dataset/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/log/__init__.py` & `inspect_ai-0.3.5/src/inspect_ai/log/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/log/_file.py` & `inspect_ai-0.3.5/src/inspect_ai/log/_file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/log/_log.py` & `inspect_ai-0.3.5/src/inspect_ai/log/_log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/__init__.py` & `inspect_ai-0.3.5/src/inspect_ai/model/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_model.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,18 +341,19 @@
 
         Args:
           completion (str): Text for first message.
         """
         if len(self.choices) > 0:
             self.choices[0].message.text = completion
         else:
-            self.choices.append(ChatCompletionChoice(
-                message = ChatMessageAssistant(content = completion),
-                stop_reason="stop"
-            ))
+            self.choices.append(
+                ChatCompletionChoice(
+                    message=ChatMessageAssistant(content=completion), stop_reason="stop"
+                )
+            )
 
     @staticmethod
     def from_content(
         model: str,
         content: str,
         stop_reason: StopReason = "stop",
         error: str | None = None,
@@ -673,15 +674,15 @@
             return (None, model)
 
 
 def get_model(
     model: str | Model | None = None,
     config: GenerateConfig = GenerateConfig(),
     base_url: str | None = None,
-    **model_args: dict[str, Any],
+    **model_args: Any,
 ) -> Model:
     """Get an instance of a model.
 
     Args:
        model (str | Model | None): Model specification.
          If `Model` is passed it is returned unmodified,
          if `None` is passed then the model currently being
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/anthropic.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/azureai.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/azureai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/bedrock.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/bedrock.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/cloudflare.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/google.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/google.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/hf.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/hf.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from queue import Empty, Queue
 from threading import Thread
 from typing import Any, Literal, Protocol, cast
 
 import numpy as np
 import torch
 from torch import Tensor
-from transformers import AutoModelForCausalLM, AutoTokenizer, set_seed  # type: ignore
+from transformers import (  # type: ignore
+    AutoModelForCausalLM,
+    AutoTokenizer,
+    set_seed,
+)
 from typing_extensions import override
 
 from inspect_ai._util.constants import DEFAULT_MAX_TOKENS
 
 from .._model import (
     ChatCompletionChoice,
     ChatMessage,
@@ -51,14 +55,15 @@
             return value
 
         device = collect_model_arg("device")
         tokenizer = collect_model_arg("tokenizer")
         model_path = collect_model_arg("model_path")
         tokenizer_path = collect_model_arg("tokenizer_path")
         self.batch_size = collect_model_arg("batch_size")
+        self.chat_template = collect_model_arg("chat_template")
 
         # device
         if device:
             self.device = device
         elif torch.backends.mps.is_available():
             self.device = "mps"
         elif torch.cuda.is_available():
@@ -84,14 +89,15 @@
                 self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_path)
             else:
                 self.tokenizer = AutoTokenizer.from_pretrained(model_path)
         else:
             self.tokenizer = AutoTokenizer.from_pretrained(model_name)
         # LLMs generally don't have a pad token and we need one for batching
         self.tokenizer.pad_token = self.tokenizer.eos_token
+        self.tokenizer.padding_side = "left"
 
     async def generate(
         self,
         input: list[ChatMessage],
         tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
@@ -125,14 +131,15 @@
         response = await batched_generate(
             GenerateInput(
                 input=chat,
                 device=self.device,
                 tokenizer=tokenizer,
                 generator=generator,
                 decoder=decoder,
+                batch_size=config.max_connections or self.max_connections(),
             )
         )
 
         # construct choice
         choice = ChatCompletionChoice(
             message=ChatMessageAssistant(content=response.output, source="generate")
         )
@@ -161,78 +168,87 @@
     def hf_chat(self, messages: list[ChatMessage]) -> str:
         # handle system message and consecutive user messages
         messages = simple_input_messages(messages)
         # convert to hf format
         hf_messages = chat_api_input(messages)
         # apply chat template
         chat = self.tokenizer.apply_chat_template(
-            hf_messages, add_generation_prompt=True, tokenize=False
+            hf_messages,
+            add_generation_prompt=True,
+            tokenize=False,
+            chat_template=self.chat_template,
         )
-
         # return
         return cast(str, chat)
 
 
 def set_random_seeds(seed: int | None = None) -> None:
     if seed is None:
         seed = np.random.default_rng().integers(2**32 - 1)
     # python hash seed
     os.environ["PYTHONHASHSEED"] = str(seed)
     # transformers seed
     set_seed(seed)
 
 
 class Tokenizer(Protocol):
-    def __call__(self, input: list[str]) -> dict[Literal["input_ids"], Tensor]:
-        ...
+    def __call__(
+        self, input: list[str]
+    ) -> dict[Literal["input_ids", "attention_mask"], Tensor]: ...
 
 
 class Generator(Protocol):
-    def __call__(self, input_ids: Tensor) -> Tensor:
-        ...
+    def __call__(self, input_ids: Tensor, attention_mask: Tensor) -> Tensor: ...
 
 
 class Decoder(Protocol):
-    def __call__(self, sequences: Tensor) -> list[str]:
-        ...
+    def __call__(self, sequences: Tensor) -> list[str]: ...
 
 
 @dataclass
 class GenerateInput:
     input: str
     device: str
     tokenizer: Tokenizer
     generator: Generator
     decoder: Decoder
+    batch_size: int
 
 
 @dataclass
 class GenerateOutput:
     output: str
     input_tokens: int
     output_tokens: int
     total_tokens: int
 
 
+@dataclass
+class _QueueItem:
+    input: GenerateInput
+    future: asyncio.Future[GenerateOutput]
+    loop: asyncio.AbstractEventLoop
+
+
 batch_thread: Thread | None = None
 
-batch_queue: "Queue[tuple[GenerateInput, asyncio.Future[GenerateOutput]]]" = Queue()
+batch_queue: "Queue[_QueueItem]" = Queue()
 
 
 async def batched_generate(input: GenerateInput) -> GenerateOutput:
     # start the background thread if necessary
     global batch_thread
     if batch_thread is None:
         batch_thread = Thread(target=process_batches, daemon=True)
         batch_thread.start()
 
     # enque the job
     loop = asyncio.get_event_loop()
     future: asyncio.Future[GenerateOutput] = loop.create_future()
-    batch_queue.put((input, future))
+    batch_queue.put(_QueueItem(input=input, future=future, loop=loop))
 
     # await the job
     await future
 
     # return it
     return future.result()
 
@@ -240,16 +256,21 @@
 def process_batches() -> None:
     while True:
         # drain the queue (wait until no new messages have shown up for 2 secones)
         inputs: list[tuple[GenerateInput, asyncio.Future[GenerateOutput]]] = []
         while True:
             try:
                 input = batch_queue.get(timeout=2)
-                inputs.append(input)
+                loop = input.loop
+                inputs.append((input.input, input.future))
+                if len(inputs) == input.input.batch_size:
+                    # max batch size reached
+                    break
             except Empty:
+                # we have exhausted the queue
                 break
 
         # see if we have any work to do
         if len(inputs) == 0:
             continue
 
         try:
@@ -257,34 +278,45 @@
             first_input = inputs[0][0]
             device = first_input.device
             tokenizer = first_input.tokenizer
             generator = first_input.generator
             decoder = first_input.decoder
 
             # tokenize and move to device
-            input_ids = tokenizer([item[0].input for item in inputs])["input_ids"]
+            tokenized_inputs = tokenizer([item[0].input for item in inputs])
+            input_ids = tokenized_inputs["input_ids"]
+            attention_mask = tokenized_inputs["attention_mask"]
             input_ids = input_ids.to(device)
+            attention_mask = attention_mask.to(device)
 
             # generate
             with torch.inference_mode():
-                generate_ids = generator(input_ids=input_ids)
+                generate_ids = generator(
+                    input_ids=input_ids, attention_mask=attention_mask
+                )
 
             # decode
             outputs = decoder(sequences=generate_ids[:, input_ids.size(dim=1) :])
 
             # call back futures
             for i, output in enumerate(outputs):
                 future = inputs[i][1]
                 input_tokens = input_ids.size(dim=1)
                 output_tokens = generate_ids.size(dim=1) - input_ids.size(dim=1)
-                future.set_result(
+
+                # asyncio futures are not thread safe, so we need to pass the event loop
+                # down to this point, so we can mark the future as done in a thread safe manner.
+                # see: https://docs.python.org/3/library/asyncio-dev.html#concurrency-and-multithreading
+                loop.call_soon_threadsafe(
+                    future.set_result,
                     GenerateOutput(
                         output=output,
                         input_tokens=input_tokens,
                         output_tokens=output_tokens,
                         total_tokens=input_tokens + output_tokens,
-                    )
+                    ),
                 )
+
         except Exception as ex:
-            for input in inputs:
-                future = input[1]
-                future.set_exception(ex)
+            for inp in inputs:
+                future = inp[1]
+                loop.call_soon_threadsafe(future.set_exception, ex)
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/mistral.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/mistral.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 raise ValueError(
                     f"{MISTRAL_API_KEY} or {AZUREAI_MISTRAL_API_KEY} environment variable not found."
                 )
             base_url = model_base_url(base_url, "AZUREAI_MISTRAL_BASE_URL")
             if not base_url:
                 raise ValueError(
                     "You must provide a base URL when using Mistral on Azure. Use the AZUREAI_MISTRAL_BASE_URL "
-                    + " environment variable or the --model_base_url CLI flag to set the base URL."
+                    + " environment variable or the --model-base-url CLI flag to set the base URL."
                 )
             model_args["endpoint"] = base_url
 
         # save key
         self.api_key = api_key
 
         # create client
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/openai.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                     "AZURE_OPENAI_BASE_URL",
                     "AZURE_OPENAI_ENDPOINT",
                 ],
             )
             if not base_url:
                 raise ValueError(
                     "You must provide a base URL when using OpenAI on Azure. Use the AZUREAI_OPENAI_BASE_URL "
-                    + " environment variable or the --model_base_url CLI flag to set the base URL."
+                    + " environment variable or the --model-base-url CLI flag to set the base URL."
                 )
 
             self.client: AsyncAzureOpenAI | AsyncOpenAI = AsyncAzureOpenAI(
                 api_key=api_key,
                 azure_endpoint=base_url,
                 azure_deployment=model_name,
                 max_retries=(
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/providers.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/providers.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/together.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/together.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_providers/util.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_providers/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_registry.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_tool.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/model/_util.py` & `inspect_ai-0.3.5/src/inspect_ai/model/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/__init__.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_answer.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_answer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_common.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_match.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_match.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_metric.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/accuracy.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/mean.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/mean.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/std.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/std.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_model.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_model.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_pattern.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_pattern.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/scorer/_scorer.py` & `inspect_ai-0.3.5/src/inspect_ai/scorer/_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/__init__.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_critique.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_critique.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_multiple_choice.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_multiple_choice.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_plan.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_prompt.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_prompt.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_solver.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool_def.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool_def.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/use_tools.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/use_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/web_search.py` & `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/web_search.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/util/_context/concurrency.py` & `inspect_ai-0.3.5/src/inspect_ai/util/_context/concurrency.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/util/_context/logger.py` & `inspect_ai-0.3.5/src/inspect_ai/util/_context/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/util/_context/resource.py` & `inspect_ai-0.3.5/src/inspect_ai/util/_context/resource.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai/util/_context/subprocess.py` & `inspect_ai-0.3.5/src/inspect_ai/util/_context/subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/src/inspect_ai.egg-info/PKG-INFO` & `inspect_ai-0.3.5/src/inspect_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.4
+Version: 0.3.5
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
@@ -60,14 +60,15 @@
 Requires-Dist: openai; extra == "dev"
 Requires-Dist: anthropic; extra == "dev"
 Requires-Dist: google-cloud-aiplatform; extra == "dev"
 Requires-Dist: google-generativeai; extra == "dev"
 Requires-Dist: mistralai; extra == "dev"
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: transformers; extra == "dev"
+Requires-Dist: accelerate; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: datasets; extra == "dev"
 Requires-Dist: langchain; extra == "dev"
 Requires-Dist: langchainhub; extra == "dev"
 Requires-Dist: wikipedia; extra == "dev"
 Requires-Dist: ipywidgets; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai.egg-info/SOURCES.txt` & `inspect_ai-0.3.5/src/inspect_ai.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -265,14 +265,15 @@
 src/inspect_ai/util/_context/subprocess.py
 tests/test_anthropic.py
 tests/test_cloudlfare.py
 tests/test_collapse_user_message.py
 tests/test_dataset.py
 tests/test_eval_log.py
 tests/test_examples.py
+tests/test_hf.py
 tests/test_images.py
 tests/test_list_task.py
 tests/test_logprobs.py
 tests/test_metric.py
 tests/test_num_choices.py
 tests/test_openai.py
 tests/test_plan.py
```

### Comparing `inspect_ai-0.3.4/src/inspect_ai.egg-info/requires.txt` & `inspect_ai-0.3.5/src/inspect_ai.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 openai
 anthropic
 google-cloud-aiplatform
 google-generativeai
 mistralai
 boto3
 transformers
+accelerate
 torch
 datasets
 langchain
 langchainhub
 wikipedia
 ipywidgets
 ipython
```

### Comparing `inspect_ai-0.3.4/tests/test_anthropic.py` & `inspect_ai-0.3.5/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_collapse_user_message.py` & `inspect_ai-0.3.5/tests/test_collapse_user_message.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_dataset.py` & `inspect_ai-0.3.5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_eval_log.py` & `inspect_ai-0.3.5/tests/test_eval_log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_images/images.jsonl` & `inspect_ai-0.3.5/tests/test_images/images.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_images.py` & `inspect_ai-0.3.5/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_list_task.py` & `inspect_ai-0.3.5/tests/test_list_task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_logprobs.py` & `inspect_ai-0.3.5/tests/test_logprobs.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_metric.py` & `inspect_ai-0.3.5/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_num_choices.py` & `inspect_ai-0.3.5/tests/test_num_choices.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_openai.py` & `inspect_ai-0.3.5/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_plan.py` & `inspect_ai-0.3.5/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_registry.py` & `inspect_ai-0.3.5/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_retry.py` & `inspect_ai-0.3.5/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_scorer.py` & `inspect_ai-0.3.5/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_solver.py` & `inspect_ai-0.3.5/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_stop_reason.py` & `inspect_ai-0.3.5/tests/test_stop_reason.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_subprocess.py` & `inspect_ai-0.3.5/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/test_tools.py` & `inspect_ai-0.3.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.4/tests/utils.py` & `inspect_ai-0.3.5/tests/utils.py`

 * *Files identical despite different names*

