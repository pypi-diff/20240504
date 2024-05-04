# Comparing `tmp/py_dbchat-0.0.2rc98.post1.tar.gz` & `tmp/py_dbchat-0.0.2rc99.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dbchat-0.0.2rc98.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_dbchat-0.0.2rc99.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_dbchat-0.0.2rc98.post1.tar` & `py_dbchat-0.0.2rc99.post1.tar`

### file list

```diff
@@ -1,122 +1,124 @@
--rw-r--r--   0        0        0   600200 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.devcontainer/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      462 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1822 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      950 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0      417 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.gitignore
--rw-r--r--   0        0        0     1381 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.pypirc
--rw-r--r--   0        0        0      791 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1213 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/LICENSE
--rw-r--r--   0        0        0       41 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/README.md
--rw-r--r--   0        0        0     2780 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/SUPPORT.md
--rw-r--r--   0        0        0      655 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/Test.session.sql
--rw-r--r--   0        0        0      634 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/docs/make.bat
--rw-r--r--   0        0        0       50 2024-04-27 12:51:28.530731 py_dbchat-0.0.2rc98.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/pyproject.md
--rw-r--r--   0        0        0      423 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/python_package.rst
--rw-r--r--   0        0        0       65 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/docs/workflows.md
--rw-r--r--   0        0        0     3399 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/package-lock.json
--rw-r--r--   0        0        0       62 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/package.json
--rw-r--r--   0        0        0      203 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/playground.py
--rw-r--r--   0        0        0     6679 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/pyproject.toml
--rw-r--r--   0        0        0      101 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/requirements.txt
--rw-r--r--   0        0        0      109 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/README.md
--rw-r--r--   0        0        0      161 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/Roadmap.md
--rw-r--r--   0        0        0        0 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/__init__.py
--rw-r--r--   0        0        0       41 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/.env.sample
--rw-r--r--   0        0        0        0 2024-04-27 12:51:40.878703 py_dbchat-0.0.2rc98.post1/src/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/agents/agent.py
--rw-r--r--   0        0        0      825 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/agents/chat_manager.py
--rw-r--r--   0        0        0     3553 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/database/repository.py
--rw-r--r--   0        0        0      637 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/dependencies.py
--rw-r--r--   0        0        0        0 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/internal/__init__.py
--rw-r--r--   0        0        0      146 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/internal/admin.py
--rw-r--r--   0        0        0     1051 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/main.py
--rw-r--r--   0        0        0      562 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/models/AppSettings.py
--rw-r--r--   0        0        0       79 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/models/BaseDbModel.py
--rw-r--r--   0        0        0      427 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/models/Connections.py
--rw-r--r--   0        0        0        0 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/models/__init__.py
--rw-r--r--   0        0        0      552 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/models/model_map.py
--rw-r--r--   0        0        0        0 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/routers/__init__.py
--rw-r--r--   0        0        0     2122 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/routers/connections.py
--rw-r--r--   0        0        0     3472 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/routers/conversation.py
--rw-r--r--   0        0        0     1010 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/routers/items.py
--rw-r--r--   0        0        0     1319 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/routers/settings.py
--rw-r--r--   0        0        0      406 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/routers/users.py
--rw-r--r--   0        0        0      390 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/api/settings.py
--rw-r--r--   0        0        0     6148 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/.DS_Store
--rw-r--r--   0        0        0      374 2024-04-27 12:51:40.878703 py_dbchat-0.0.2rc98.post1/src/db_chat/__init__.py
--rw-r--r--   0        0        0      725 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/ask.py
--rw-r--r--   0        0        0      662 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/hello_world.py
--rw-r--r--   0        0        0     3833 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/llm/classic_prompt.py
--rw-r--r--   0        0        0     3518 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/llm/function_calling.py
--rw-r--r--   0        0        0     6791 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/llm/llm.py
--rw-r--r--   0        0        0     1135 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/llm/llm_langchain_sample.py
--rw-r--r--   0        0        0      250 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/Filter.py
--rw-r--r--   0        0        0      236 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/FilterOperator.py
--rw-r--r--   0        0        0     2478 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/Query.py
--rw-r--r--   0        0        0      159 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/SortOrder.py
--rw-r--r--   0        0        0        0 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/__init__.py
--rw-r--r--   0        0        0      453 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/mappings.py
--rw-r--r--   0        0        0     5198 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/schema.py
--rw-r--r--   0        0        0     8781 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/sql_builder.py
--rw-r--r--   0        0        0    16036 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
--rw-r--r--   0        0        0      436 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/.eslintrc.cjs
--rw-r--r--   0        0        0      253 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/.gitignore
--rw-r--r--   0        0        0     1300 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/README.md
--rw-r--r--   0        0        0      483 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/index.html
--rw-r--r--   0        0        0   120043 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/package-lock.json
--rw-r--r--   0        0        0      944 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/package.json
--rw-r--r--   0        0        0     1497 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/public/vite.svg
--rw-r--r--   0        0        0     1667 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/App.css
--rw-r--r--   0        0        0     1727 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/App.tsx
--rw-r--r--   0        0        0     3202 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/api/baseApi.ts
--rw-r--r--   0        0        0        0 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/api/conversationApi.ts
--rw-r--r--   0        0        0     4126 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/assets/react.svg
--rw-r--r--   0        0        0     2435 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/components/menu/menu.tsx
--rw-r--r--   0        0        0     1161 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/index.css
--rw-r--r--   0        0        0      235 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/main.tsx
--rw-r--r--   0        0        0     4195 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/pages/connections/connections.tsx
--rw-r--r--   0        0        0     5262 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/pages/home/home.tsx
--rw-r--r--   0        0        0     2167 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/pages/settings/settings.tsx
--rw-r--r--   0        0        0     1202 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/store/appSettingStore.ts
--rw-r--r--   0        0        0     5187 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/store/chatConversationStore.ts
--rw-r--r--   0        0        0     3309 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/store/connectionsStore.ts
--rw-r--r--   0        0        0      624 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/store/uiStore.ts
--rw-r--r--   0        0        0       83 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/types/Setting.ts
--rw-r--r--   0        0        0       40 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/types/index.ts
--rw-r--r--   0        0        0       84 2024-04-27 12:51:28.534731 py_dbchat-0.0.2rc98.post1/src/ui/src/types/menu.ts
--rw-r--r--   0        0        0       64 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/src/ui/src/types/schema.ts
--rw-r--r--   0        0        0       38 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/src/ui/src/vite-env.d.ts
--rw-r--r--   0        0        0      605 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/src/ui/tsconfig.json
--rw-r--r--   0        0        0      233 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/src/ui/tsconfig.node.json
--rw-r--r--   0        0        0      167 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/src/ui/vite.config.ts
--rw-r--r--   0        0        0   600200 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/test/Chinook_PostgreSql.sql
--rw-r--r--   0        0        0      989 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/tests/conftest.py
--rw-r--r--   0        0        0     2922 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/tests/test_explicit_joins.py
--rw-r--r--   0        0        0     1210 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/tests/test_methods.py
--rw-r--r--   0        0        0      269 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/tests/test_schema_builder.py
--rw-r--r--   0        0        0    12288 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/tests/test_sql_builder.py
--rw-r--r--   0        0        0     7124 2024-04-27 12:51:28.538731 py_dbchat-0.0.2rc98.post1/tests/test_sqlalchemy.py
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc98.post1/PKG-INFO
+-rw-r--r--   0        0        0   600200 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.devcontainer/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      462 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1822 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      950 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0      417 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.gitignore
+-rw-r--r--   0        0        0     1381 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.pypirc
+-rw-r--r--   0        0        0      791 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1213 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/LICENSE
+-rw-r--r--   0        0        0       41 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/README.md
+-rw-r--r--   0        0        0     2780 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/SUPPORT.md
+-rw-r--r--   0        0        0      655 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/Test.session.sql
+-rw-r--r--   0        0        0      634 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-29 04:20:09.583500 py_dbchat-0.0.2rc99.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/make.bat
+-rw-r--r--   0        0        0       50 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      423 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       65 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/docs/workflows.md
+-rw-r--r--   0        0        0     3399 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/package-lock.json
+-rw-r--r--   0        0        0       62 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/package.json
+-rw-r--r--   0        0        0      203 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/playground.py
+-rw-r--r--   0        0        0     6679 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/requirements.txt
+-rw-r--r--   0        0        0      109 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/README.md
+-rw-r--r--   0        0        0      161 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/Roadmap.md
+-rw-r--r--   0        0        0        0 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/__init__.py
+-rw-r--r--   0        0        0       41 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/.env.sample
+-rw-r--r--   0        0        0        0 2024-04-29 04:20:21.863534 py_dbchat-0.0.2rc99.post1/src/api/__init__.py
+-rw-r--r--   0        0        0      894 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/agents/agent.py
+-rw-r--r--   0        0        0      170 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/agents/agent_strategy.md
+-rw-r--r--   0        0        0     4717 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/agents/autogen/react_agents.py
+-rw-r--r--   0        0        0     1879 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/agents/chat_manager.py
+-rw-r--r--   0        0        0     3553 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/database/repository.py
+-rw-r--r--   0        0        0      637 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/internal/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/internal/admin.py
+-rw-r--r--   0        0        0     1052 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/main.py
+-rw-r--r--   0        0        0      677 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/models/AppSettings.py
+-rw-r--r--   0        0        0       79 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/models/BaseDbModel.py
+-rw-r--r--   0        0        0      427 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/models/Connections.py
+-rw-r--r--   0        0        0       27 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/models/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/models/model_map.py
+-rw-r--r--   0        0        0        0 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/routers/__init__.py
+-rw-r--r--   0        0        0     2122 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/routers/connections.py
+-rw-r--r--   0        0        0     3472 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/routers/conversation.py
+-rw-r--r--   0        0        0     1010 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/routers/items.py
+-rw-r--r--   0        0        0     1319 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/routers/settings.py
+-rw-r--r--   0        0        0      406 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/routers/users.py
+-rw-r--r--   0        0        0      390 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/api/settings.py
+-rw-r--r--   0        0        0     6148 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/.DS_Store
+-rw-r--r--   0        0        0      374 2024-04-29 04:20:21.863534 py_dbchat-0.0.2rc99.post1/src/db_chat/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/ask.py
+-rw-r--r--   0        0        0      662 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/hello_world.py
+-rw-r--r--   0        0        0     3833 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/llm/classic_prompt.py
+-rw-r--r--   0        0        0     3518 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/llm/function_calling.py
+-rw-r--r--   0        0        0     6791 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/llm/llm.py
+-rw-r--r--   0        0        0     1135 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/llm/llm_langchain_sample.py
+-rw-r--r--   0        0        0      250 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/Filter.py
+-rw-r--r--   0        0        0      236 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/FilterOperator.py
+-rw-r--r--   0        0        0     2478 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/Query.py
+-rw-r--r--   0        0        0      159 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/SortOrder.py
+-rw-r--r--   0        0        0        0 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/__init__.py
+-rw-r--r--   0        0        0      453 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/mappings.py
+-rw-r--r--   0        0        0     5198 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/schema.py
+-rw-r--r--   0        0        0     8781 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/sql_builder.py
+-rw-r--r--   0        0        0    16036 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
+-rw-r--r--   0        0        0      436 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/.eslintrc.cjs
+-rw-r--r--   0        0        0      253 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/.gitignore
+-rw-r--r--   0        0        0     1300 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/README.md
+-rw-r--r--   0        0        0      483 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/index.html
+-rw-r--r--   0        0        0   120043 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/package-lock.json
+-rw-r--r--   0        0        0      944 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/package.json
+-rw-r--r--   0        0        0     1497 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/public/vite.svg
+-rw-r--r--   0        0        0     1667 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/App.css
+-rw-r--r--   0        0        0     1727 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/App.tsx
+-rw-r--r--   0        0        0     3202 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/api/baseApi.ts
+-rw-r--r--   0        0        0        0 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/api/conversationApi.ts
+-rw-r--r--   0        0        0     4126 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/assets/react.svg
+-rw-r--r--   0        0        0     2435 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/components/menu/menu.tsx
+-rw-r--r--   0        0        0     1161 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/index.css
+-rw-r--r--   0        0        0      235 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/main.tsx
+-rw-r--r--   0        0        0     4195 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/pages/connections/connections.tsx
+-rw-r--r--   0        0        0     5262 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/pages/home/home.tsx
+-rw-r--r--   0        0        0     2167 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/pages/settings/settings.tsx
+-rw-r--r--   0        0        0     1202 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/store/appSettingStore.ts
+-rw-r--r--   0        0        0     5187 2024-04-29 04:20:09.587500 py_dbchat-0.0.2rc99.post1/src/ui/src/store/chatConversationStore.ts
+-rw-r--r--   0        0        0     3309 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/src/store/connectionsStore.ts
+-rw-r--r--   0        0        0      624 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/src/store/uiStore.ts
+-rw-r--r--   0        0        0       83 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/src/types/Setting.ts
+-rw-r--r--   0        0        0       40 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/src/types/index.ts
+-rw-r--r--   0        0        0       84 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/src/types/menu.ts
+-rw-r--r--   0        0        0       64 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/src/types/schema.ts
+-rw-r--r--   0        0        0       38 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/src/vite-env.d.ts
+-rw-r--r--   0        0        0      605 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/tsconfig.node.json
+-rw-r--r--   0        0        0      167 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/src/ui/vite.config.ts
+-rw-r--r--   0        0        0   600200 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/test/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      989 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/tests/conftest.py
+-rw-r--r--   0        0        0     2922 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/tests/test_explicit_joins.py
+-rw-r--r--   0        0        0     1210 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/tests/test_methods.py
+-rw-r--r--   0        0        0      269 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/tests/test_schema_builder.py
+-rw-r--r--   0        0        0    12288 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/tests/test_sql_builder.py
+-rw-r--r--   0        0        0     7124 2024-04-29 04:20:09.591500 py_dbchat-0.0.2rc99.post1/tests/test_sqlalchemy.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc99.post1/PKG-INFO
```

### Comparing `py_dbchat-0.0.2rc98.post1/.devcontainer/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc99.post1/.devcontainer/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/.devcontainer/devcontainer.json` & `py_dbchat-0.0.2rc99.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/.devcontainer/docker-compose.yml` & `py_dbchat-0.0.2rc99.post1/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/.github/workflows/schedule-update-actions.yml` & `py_dbchat-0.0.2rc99.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/.gitignore` & `py_dbchat-0.0.2rc99.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/.pre-commit-config.yaml` & `py_dbchat-0.0.2rc99.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/.vscode/launch.json` & `py_dbchat-0.0.2rc99.post1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/.vscode/settings.json` & `py_dbchat-0.0.2rc99.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/LICENSE` & `py_dbchat-0.0.2rc99.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/SECURITY.md` & `py_dbchat-0.0.2rc99.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/SUPPORT.md` & `py_dbchat-0.0.2rc99.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/Test.session.sql` & `py_dbchat-0.0.2rc99.post1/Test.session.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/docs/Makefile` & `py_dbchat-0.0.2rc99.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/docs/conf.py` & `py_dbchat-0.0.2rc99.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/docs/make.bat` & `py_dbchat-0.0.2rc99.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/docs/pylint.md` & `py_dbchat-0.0.2rc99.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/package-lock.json` & `py_dbchat-0.0.2rc99.post1/package-lock.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/pyproject.toml` & `py_dbchat-0.0.2rc99.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/database/repository.py` & `py_dbchat-0.0.2rc99.post1/src/api/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/dependencies.py` & `py_dbchat-0.0.2rc99.post1/src/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/main.py` & `py_dbchat-0.0.2rc99.post1/src/api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
         allow_credentials=True,
         allow_methods=["*"],
         allow_headers=["*"],
+
     )
 
     app.include_router(users.router)
     app.include_router(items.router)
     app.include_router(settings.router)
     app.include_router(conversation.router)
     app.include_router(connections.router)
```

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/models/model_map.py` & `py_dbchat-0.0.2rc99.post1/src/api/models/model_map.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/routers/connections.py` & `py_dbchat-0.0.2rc99.post1/src/api/routers/connections.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/routers/conversation.py` & `py_dbchat-0.0.2rc99.post1/src/api/routers/conversation.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/routers/items.py` & `py_dbchat-0.0.2rc99.post1/src/api/routers/items.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/api/routers/settings.py` & `py_dbchat-0.0.2rc99.post1/src/api/routers/settings.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/.DS_Store` & `py_dbchat-0.0.2rc99.post1/src/db_chat/.DS_Store`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/ask.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/ask.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/hello_world.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/hello_world.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/llm/classic_prompt.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/llm/classic_prompt.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/llm/function_calling.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/llm/llm.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/llm/llm.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/llm/llm_langchain_sample.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/llm/llm_langchain_sample.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/Query.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/Query.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/schema.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/schema.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/sql_builder.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py` & `py_dbchat-0.0.2rc99.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/README.md` & `py_dbchat-0.0.2rc99.post1/src/ui/README.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/package-lock.json` & `py_dbchat-0.0.2rc99.post1/src/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/package.json` & `py_dbchat-0.0.2rc99.post1/src/ui/package.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/public/vite.svg` & `py_dbchat-0.0.2rc99.post1/src/ui/public/vite.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/App.css` & `py_dbchat-0.0.2rc99.post1/src/ui/src/App.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/App.tsx` & `py_dbchat-0.0.2rc99.post1/src/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/api/baseApi.ts` & `py_dbchat-0.0.2rc99.post1/src/ui/src/api/baseApi.ts`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/assets/react.svg` & `py_dbchat-0.0.2rc99.post1/src/ui/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/components/menu/menu.tsx` & `py_dbchat-0.0.2rc99.post1/src/ui/src/components/menu/menu.tsx`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/index.css` & `py_dbchat-0.0.2rc99.post1/src/ui/src/index.css`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/pages/connections/connections.tsx` & `py_dbchat-0.0.2rc99.post1/src/ui/src/pages/connections/connections.tsx`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/pages/home/home.tsx` & `py_dbchat-0.0.2rc99.post1/src/ui/src/pages/home/home.tsx`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/pages/settings/settings.tsx` & `py_dbchat-0.0.2rc99.post1/src/ui/src/pages/settings/settings.tsx`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/store/appSettingStore.ts` & `py_dbchat-0.0.2rc99.post1/src/ui/src/store/appSettingStore.ts`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/store/chatConversationStore.ts` & `py_dbchat-0.0.2rc99.post1/src/ui/src/store/chatConversationStore.ts`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/store/connectionsStore.ts` & `py_dbchat-0.0.2rc99.post1/src/ui/src/store/connectionsStore.ts`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/src/store/uiStore.ts` & `py_dbchat-0.0.2rc99.post1/src/ui/src/store/uiStore.ts`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/src/ui/tsconfig.json` & `py_dbchat-0.0.2rc99.post1/src/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/test/Chinook_PostgreSql.sql` & `py_dbchat-0.0.2rc99.post1/test/Chinook_PostgreSql.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/tests/conftest.py` & `py_dbchat-0.0.2rc99.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/tests/test_explicit_joins.py` & `py_dbchat-0.0.2rc99.post1/tests/test_explicit_joins.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/tests/test_methods.py` & `py_dbchat-0.0.2rc99.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/tests/test_sql_builder.py` & `py_dbchat-0.0.2rc99.post1/tests/test_sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/tests/test_sqlalchemy.py` & `py_dbchat-0.0.2rc99.post1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc98.post1/PKG-INFO` & `py_dbchat-0.0.2rc99.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbchat
-Version: 0.0.2rc98.post1
+Version: 0.0.2rc99.post1
 Summary: Chat with your existing database without using vector DB.
 Author-email: Dhanilan <mail2dhanilan@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

