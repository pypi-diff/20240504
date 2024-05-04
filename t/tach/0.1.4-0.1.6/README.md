# Comparing `tmp/tach-0.1.4.tar.gz` & `tmp/tach-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.1.4.tar", last modified: Fri May  3 01:18:31 2024, max compression
+gzip compressed data, was "tach-0.1.6.tar", last modified: Sat May  4 05:39:50 2024, max compression
```

## Comparing `tach-0.1.4.tar` & `tach-0.1.6.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.876860 tach-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.880860 tach-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 01:18:24.000000 tach-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-03 01:18:24.000000 tach-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-03 01:18:24.000000 tach-0.1.4/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-03 01:18:24.000000 tach-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 01:18:24.000000 tach-0.1.4/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-03 01:18:24.000000 tach-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-03 01:18:31.896860 tach-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-03 01:18:24.000000 tach-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 01:18:24.000000 tach-0.1.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.884860 tach-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-03 01:18:24.000000 tach-0.1.4/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-03 01:18:24.000000 tach-0.1.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-03 01:18:24.000000 tach-0.1.4/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-03 01:18:24.000000 tach-0.1.4/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 01:18:24.000000 tach-0.1.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-03 01:18:24.000000 tach-0.1.4/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-03 01:18:24.000000 tach-0.1.4/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-03 01:18:24.000000 tach-0.1.4/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-03 01:18:24.000000 tach-0.1.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 01:18:24.000000 tach-0.1.4/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-03 01:18:24.000000 tach-0.1.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-03 01:18:24.000000 tach-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 01:18:31.896860 tach-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.884860 tach-0.1.4/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-03 01:18:24.000000 tach-0.1.4/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-03 01:18:24.000000 tach-0.1.4/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-03 01:18:24.000000 tach-0.1.4/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.884860 tach-0.1.4/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-03 01:18:24.000000 tach-0.1.4/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:18:24.000000 tach-0.1.4/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 01:18:24.000000 tach-0.1.4/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:18:24.000000 tach-0.1.4/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-03 01:18:24.000000 tach-0.1.4/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:18:24.000000 tach-0.1.4/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-03 01:18:24.000000 tach-0.1.4/tach/hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-03 01:18:24.000000 tach-0.1.4/tach/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-03 01:18:24.000000 tach-0.1.4/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 01:18:24.000000 tach-0.1.4/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 01:18:24.000000 tach-0.1.4/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_module_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.592210 tach-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.600210 tach-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-04 05:39:45.000000 tach-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-04 05:39:45.000000 tach-0.1.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-04 05:39:45.000000 tach-0.1.6/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-04 05:39:45.000000 tach-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 05:39:45.000000 tach-0.1.6/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 05:39:45.000000 tach-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-04 05:39:50.612210 tach-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-04 05:39:45.000000 tach-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 05:39:45.000000 tach-0.1.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.600210 tach-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-04 05:39:45.000000 tach-0.1.6/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-04 05:39:45.000000 tach-0.1.6/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-04 05:39:45.000000 tach-0.1.6/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-04 05:39:45.000000 tach-0.1.6/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-04 05:39:45.000000 tach-0.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-04 05:39:45.000000 tach-0.1.6/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-04 05:39:45.000000 tach-0.1.6/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-04 05:39:45.000000 tach-0.1.6/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-04 05:39:45.000000 tach-0.1.6/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-04 05:39:45.000000 tach-0.1.6/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-04 05:39:45.000000 tach-0.1.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-04 05:39:45.000000 tach-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:39:50.612210 tach-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.600210 tach-0.1.6/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-04 05:39:45.000000 tach-0.1.6/tach/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-04 05:39:45.000000 tach-0.1.6/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-04 05:39:45.000000 tach-0.1.6/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.604210 tach-0.1.6/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-04 05:39:45.000000 tach-0.1.6/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-04 05:39:45.000000 tach-0.1.6/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.604210 tach-0.1.6/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-04 05:39:45.000000 tach-0.1.6/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-04 05:39:45.000000 tach-0.1.6/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.604210 tach-0.1.6/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 05:39:45.000000 tach-0.1.6/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-04 05:39:45.000000 tach-0.1.6/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-04 05:39:45.000000 tach-0.1.6/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-04 05:39:45.000000 tach-0.1.6/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.604210 tach-0.1.6/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-04 05:39:45.000000 tach-0.1.6/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-04 05:39:45.000000 tach-0.1.6/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.604210 tach-0.1.6/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 05:39:45.000000 tach-0.1.6/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-04 05:39:45.000000 tach-0.1.6/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-04 05:39:45.000000 tach-0.1.6/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 05:39:45.000000 tach-0.1.6/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-04 05:39:45.000000 tach-0.1.6/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-04 05:39:45.000000 tach-0.1.6/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.604210 tach-0.1.6/tach/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-04 05:39:45.000000 tach-0.1.6/tach/hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-04 05:39:45.000000 tach-0.1.6/tach/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-04 05:39:45.000000 tach-0.1.6/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-04 05:39:45.000000 tach-0.1.6/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-04 05:39:45.000000 tach-0.1.6/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-04 05:39:45.000000 tach-0.1.6/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-04 05:39:45.000000 tach-0.1.6/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-04 05:39:45.000000 tach-0.1.6/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-04 05:39:45.000000 tach-0.1.6/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-04 05:39:45.000000 tach-0.1.6/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-04 05:39:45.000000 tach-0.1.6/tach/parsing/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-04 05:39:50.000000 tach-0.1.6/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-04 05:39:50.000000 tach-0.1.6/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:39:50.000000 tach-0.1.6/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 05:39:50.000000 tach-0.1.6/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 05:39:50.000000 tach-0.1.6/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 05:39:50.000000 tach-0.1.6/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-04 05:39:45.000000 tach-0.1.6/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.608210 tach-0.1.6/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:39:50.612210 tach-0.1.6/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-04 05:39:45.000000 tach-0.1.6/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-04 05:39:45.000000 tach-0.1.6/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-04 05:39:45.000000 tach-0.1.6/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-04 05:39:45.000000 tach-0.1.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-04 05:39:45.000000 tach-0.1.6/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-04 05:39:45.000000 tach-0.1.6/tests/test_module_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-04 05:39:45.000000 tach-0.1.6/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:39:45.000000 tach-0.1.6/tests/test_show.py
```

### Comparing `tach-0.1.4/.github/workflows/ci.yml` & `tach-0.1.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/.github/workflows/publish.yml` & `tach-0.1.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/.github/workflows/publish_docs.yml` & `tach-0.1.6/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/.gitignore` & `tach-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/LICENSE` & `tach-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/PKG-INFO` & `tach-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.4
+Version: 0.1.6
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.1.4/README.md` & `tach-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/configuration.md` & `tach-0.1.6/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/faq.md` & `tach-0.1.6/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/favicon.ico` & `tach-0.1.6/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/getting-started.md` & `tach-0.1.6/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/index.md` & `tach-0.1.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/strict-mode.md` & `tach-0.1.6/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/tach-ignore.md` & `tach-0.1.6/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/tach_demo.mp4` & `tach-0.1.6/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/usage.md` & `tach-0.1.6/docs/usage.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/docs/why-tach.md` & `tach-0.1.6/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/mkdocs.yml` & `tach-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/pyproject.toml` & `tach-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.1.4"
+version = "0.1.6"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tach-0.1.4/tach/add.py` & `tach-0.1.6/tach/add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/check.py` & `tach-0.1.6/tach/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import re
 from dataclasses import dataclass, field
 from typing import Optional
 
 from tach import filesystem as fs
 from tach.core import PackageTrie, PackageNode, ProjectConfig
 from tach.parsing import build_package_trie, get_project_imports
 
@@ -131,18 +130,15 @@
         )
     file_tags = file_nearest_package.config.tags
     import_tags = import_nearest_package.config.tags
 
     for file_tag in file_tags:
         dependency_tags = project_config.dependencies_for_tag(file_tag)
         if any(
-            any(
-                re.match(dependency_tag, import_tag)
-                for dependency_tag in dependency_tags
-            )
+            any(dependency_tag == import_tag for dependency_tag in dependency_tags)
             for import_tag in import_tags
         ):
             # The import has at least one tag which matches at least one expected dependency
             continue
         # This means the import has no tags which the file can depend on
         return CheckResult.fail(
             error_info=ErrorInfo(
```

### Comparing `tach-0.1.4/tach/cli.py` & `tach-0.1.6/tach/cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/core/config.py` & `tach-0.1.6/tach/core/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/core/package.py` & `tach-0.1.6/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/filesystem/__init__.py` & `tach-0.1.6/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/filesystem/install.py` & `tach-0.1.6/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/filesystem/project.py` & `tach-0.1.6/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/filesystem/service.py` & `tach-0.1.6/tach/filesystem/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,30 +158,33 @@
         if dirpath == canonical_root:
             continue
 
         if exclude_hidden_paths and os.path.basename(dirpath).startswith("."):
             continue
 
         if exclude_paths is not None and any(
-            dirpath_for_matching.startswith(exclude_path)
-            or re.match(exclude_path, dirpath_for_matching)
+            re.match(exclude_path, dirpath_for_matching)
             for exclude_path in exclude_paths
         ):
             # Treat excluded paths as invisible
             continue
 
         if depth:
             # Ignore anything past requested depth
             current_depth = dirpath.count(os.path.sep)
             if current_depth >= base_depth + depth:
                 continue
         for filename in filenames:
             if exclude_hidden_paths and filename.startswith("."):
                 continue
             file_path = os.path.join(dirpath, filename)
+            if exclude_paths is not None and any(
+                re.match(exclude_path, file_path) for exclude_path in exclude_paths
+            ):
+                continue
             if filename.endswith(".py"):
                 yield file_path
 
 
 def walk_pypackages(
     root: str,
     depth: Optional[int] = None,
```

### Comparing `tach-0.1.4/tach/init.py` & `tach-0.1.6/tach/init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/loading.py` & `tach-0.1.6/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/parsing/config.py` & `tach-0.1.6/tach/parsing/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/parsing/imports.py` & `tach-0.1.6/tach/parsing/imports.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/parsing/interface.py` & `tach-0.1.6/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach/parsing/packages.py` & `tach-0.1.6/tach/parsing/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tach.egg-info/PKG-INFO` & `tach-0.1.6/tach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.4
+Version: 0.1.6
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.1.4/tach.egg-info/SOURCES.txt` & `tach-0.1.6/tach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tests/test_add.py` & `tach-0.1.6/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tests/test_check.py` & `tach-0.1.6/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tests/test_cli.py` & `tach-0.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tests/test_init.py` & `tach-0.1.6/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tests/test_module_trie.py` & `tach-0.1.6/tests/test_module_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.4/tests/test_parsing.py` & `tach-0.1.6/tests/test_parsing.py`

 * *Files identical despite different names*

