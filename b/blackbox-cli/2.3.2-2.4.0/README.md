# Comparing `tmp/blackbox_cli-2.3.2.tar.gz` & `tmp/blackbox_cli-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackbox_cli-2.3.2.tar", max compression
+gzip compressed data, was "blackbox_cli-2.4.0.tar", max compression
```

## Comparing `blackbox_cli-2.3.2.tar` & `blackbox_cli-2.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1071 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/LICENSE
--rw-r--r--   0        0        0    17439 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/README.md
--rw-r--r--   0        0        0      129 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/__init__.py
--rw-r--r--   0        0        0      148 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/__main__.py
--rw-r--r--   0        0        0     6044 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/cli.py
--rw-r--r--   0        0        0     4369 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/config.py
--rw-r--r--   0        0        0     1352 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/exceptions.py
--rw-r--r--   0        0        0      117 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/__init__.py
--rw-r--r--   0        0        0     1081 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/_base.py
--rw-r--r--   0        0        0      214 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/__init__.py
--rw-r--r--   0        0        0     1124 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/_base.py
--rw-r--r--   0        0        0     1539 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/localstorage.py
--rw-r--r--   0        0        0     1147 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/mariadb.py
--rw-r--r--   0        0        0      969 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/mongodb.py
--rw-r--r--   0        0        0      251 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/mysql.py
--rw-r--r--   0        0        0      848 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/postgres.py
--rw-r--r--   0        0        0      803 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/databases/redis.py
--rw-r--r--   0        0        0      121 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/notifiers/__init__.py
--rw-r--r--   0        0        0      885 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/notifiers/_base.py
--rw-r--r--   0        0        0     2317 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/notifiers/discord.py
--rw-r--r--   0        0        0     5118 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/notifiers/slack.py
--rw-r--r--   0        0        0     1568 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/notifiers/telegram.py
--rw-r--r--   0        0        0       83 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/storage/__init__.py
--rw-r--r--   0        0        0     2383 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/storage/_base.py
--rw-r--r--   0        0        0     5359 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/storage/dropbox.py
--rw-r--r--   0        0        0     4964 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/handlers/storage/s3.py
--rw-r--r--   0        0        0       62 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/__init__.py
--rw-r--r--   0        0        0     1262 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/commands.py
--rw-r--r--   0        0        0     2329 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/cooldown.py
--rw-r--r--   0        0        0      339 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/logger.py
--rw-r--r--   0        0        0     1499 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/mixins.py
--rw-r--r--   0        0        0     1647 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/reports.py
--rw-r--r--   0        0        0     4152 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/workflows.py
--rw-r--r--   0        0        0     1393 2023-03-02 20:16:02.807489 blackbox_cli-2.3.2/blackbox/utils/yaml.py
--rw-r--r--   0        0        0     1549 2023-03-02 20:16:02.811489 blackbox_cli-2.3.2/pyproject.toml
--rw-r--r--   0        0        0    19212 1970-01-01 00:00:00.000000 blackbox_cli-2.3.2/setup.py
--rw-r--r--   0        0        0    18728 1970-01-01 00:00:00.000000 blackbox_cli-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/LICENSE
+-rw-r--r--   0        0        0    17439 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/README.md
+-rw-r--r--   0        0        0      129 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/__main__.py
+-rw-r--r--   0        0        0     6044 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/cli.py
+-rw-r--r--   0        0        0     4369 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/config.py
+-rw-r--r--   0        0        0     1352 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/exceptions.py
+-rw-r--r--   0        0        0      117 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/handlers/__init__.py
+-rw-r--r--   0        0        0     1081 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/handlers/_base.py
+-rw-r--r--   0        0        0      214 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/handlers/databases/__init__.py
+-rw-r--r--   0        0        0     1124 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/handlers/databases/_base.py
+-rw-r--r--   0        0        0     1539 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/handlers/databases/localstorage.py
+-rw-r--r--   0        0        0     1147 2024-05-04 00:44:43.360421 blackbox_cli-2.4.0/blackbox/handlers/databases/mariadb.py
+-rw-r--r--   0        0        0      969 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/databases/mongodb.py
+-rw-r--r--   0        0        0      251 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/databases/mysql.py
+-rw-r--r--   0        0        0      848 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/databases/postgres.py
+-rw-r--r--   0        0        0      803 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/databases/redis.py
+-rw-r--r--   0        0        0      121 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/notifiers/__init__.py
+-rw-r--r--   0        0        0      885 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/notifiers/_base.py
+-rw-r--r--   0        0        0     2317 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/notifiers/discord.py
+-rw-r--r--   0        0        0     5118 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/notifiers/slack.py
+-rw-r--r--   0        0        0     1568 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/notifiers/telegram.py
+-rw-r--r--   0        0        0       83 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/storage/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/storage/_base.py
+-rw-r--r--   0        0        0     5359 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/storage/dropbox.py
+-rw-r--r--   0        0        0     4964 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/handlers/storage/s3.py
+-rw-r--r--   0        0        0       62 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/commands.py
+-rw-r--r--   0        0        0     2329 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/cooldown.py
+-rw-r--r--   0        0        0      339 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/logger.py
+-rw-r--r--   0        0        0     1499 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/mixins.py
+-rw-r--r--   0        0        0     1647 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/reports.py
+-rw-r--r--   0        0        0     4152 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/workflows.py
+-rw-r--r--   0        0        0     1393 2024-05-04 00:44:43.364421 blackbox_cli-2.4.0/blackbox/utils/yaml.py
+-rw-r--r--   0        0        0     1557 2024-05-04 00:44:43.368421 blackbox_cli-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    19212 1970-01-01 00:00:00.000000 blackbox_cli-2.4.0/setup.py
+-rw-r--r--   0        0        0    18728 1970-01-01 00:00:00.000000 blackbox_cli-2.4.0/PKG-INFO
```

### Comparing `blackbox_cli-2.3.2/LICENSE` & `blackbox_cli-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/README.md` & `blackbox_cli-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/cli.py` & `blackbox_cli-2.4.0/blackbox/cli.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/config.py` & `blackbox_cli-2.4.0/blackbox/config.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/exceptions.py` & `blackbox_cli-2.4.0/blackbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/_base.py` & `blackbox_cli-2.4.0/blackbox/handlers/_base.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/databases/_base.py` & `blackbox_cli-2.4.0/blackbox/handlers/databases/_base.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/databases/localstorage.py` & `blackbox_cli-2.4.0/blackbox/handlers/databases/localstorage.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/databases/mariadb.py` & `blackbox_cli-2.4.0/blackbox/handlers/databases/mariadb.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/databases/mongodb.py` & `blackbox_cli-2.4.0/blackbox/handlers/databases/mongodb.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/databases/postgres.py` & `blackbox_cli-2.4.0/blackbox/handlers/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/databases/redis.py` & `blackbox_cli-2.4.0/blackbox/handlers/databases/redis.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/notifiers/_base.py` & `blackbox_cli-2.4.0/blackbox/handlers/notifiers/_base.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/notifiers/discord.py` & `blackbox_cli-2.4.0/blackbox/handlers/notifiers/discord.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/notifiers/slack.py` & `blackbox_cli-2.4.0/blackbox/handlers/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/notifiers/telegram.py` & `blackbox_cli-2.4.0/blackbox/handlers/notifiers/telegram.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/storage/_base.py` & `blackbox_cli-2.4.0/blackbox/handlers/storage/_base.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/storage/dropbox.py` & `blackbox_cli-2.4.0/blackbox/handlers/storage/dropbox.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/handlers/storage/s3.py` & `blackbox_cli-2.4.0/blackbox/handlers/storage/s3.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/utils/commands.py` & `blackbox_cli-2.4.0/blackbox/utils/commands.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/utils/cooldown.py` & `blackbox_cli-2.4.0/blackbox/utils/cooldown.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/utils/mixins.py` & `blackbox_cli-2.4.0/blackbox/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/utils/reports.py` & `blackbox_cli-2.4.0/blackbox/utils/reports.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/utils/workflows.py` & `blackbox_cli-2.4.0/blackbox/utils/workflows.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/blackbox/utils/yaml.py` & `blackbox_cli-2.4.0/blackbox/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `blackbox_cli-2.3.2/pyproject.toml` & `blackbox_cli-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "blackbox-cli"
 packages = [
     { include = "blackbox" }
 ]
-version = "v2.3.2"
+version = "v2.4.0"
 description = "Tool for automatic backups of databases"
 authors = ["Leon Sandøy <leon.sandoy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lemonsaurus/blackbox"
 repository = "https://github.com/lemonsaurus/blackbox"
 classifiers = [
@@ -24,15 +24,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^5.3.1"
 requests = "^2.25.1"
 boto3 = "^1.16.51"
 loguru = "^0.5.3"
 jinja2 = "^3.1.2"
-click = "^7.1.2"
+click = ">=7.1.2,<9.0.0"
 dropbox = "^11.0.0"
 pytelegrambotapi = "^3.7.7"
 single-source = "^0.2.0"
 stone = "^3.2.1"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.9.2"
```

### Comparing `blackbox_cli-2.3.2/setup.py` & `blackbox_cli-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,30 +10,30 @@
  'blackbox.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.16.51,<2.0.0',
- 'click>=7.1.2,<8.0.0',
+ 'click>=7.1.2,<9.0.0',
  'dropbox>=11.0.0,<12.0.0',
  'jinja2>=3.1.2,<4.0.0',
  'loguru>=0.5.3,<0.6.0',
  'pytelegrambotapi>=3.7.7,<4.0.0',
  'pyyaml>=5.3.1,<6.0.0',
  'requests>=2.25.1,<3.0.0',
  'single-source>=0.2.0,<0.3.0',
  'stone>=3.2.1,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['blackbox = blackbox.cli:cli']}
 
 setup_kwargs = {
     'name': 'blackbox-cli',
-    'version': '2.3.2',
+    'version': '2.4.0',
     'description': 'Tool for automatic backups of databases',
     'long_description': '![Lint & Test](https://github.com/lemonsaurus/blackbox/workflows/Lint%20&%20Test/badge.svg)\n![Docker Build](https://github.com/lemonsaurus/blackbox/workflows/Docker%20Build/badge.svg)\n[![PyPI version](https://badge.fury.io/py/blackbox-cli.svg)](https://pypi.org/project/blackbox-cli/)\n\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_banner.png)\n\nA simple service which magically backs up all your databases to all your\nfavorite cloud storage providers, and then notifies you.\n\nSimply create a config file, fill in some connection strings for your favorite\nservices, and schedule `blackbox` to run however often you want using something\nlike `cron`, or a Kubernetes CronJob.\n\n## Table of Contents\n\n- [Setup](#setup)\n- [Configuration](#configuration)\n- [Environment Variables](#environment-variables)\n- [Databases](#databases)\n    - [MongoDB](#mongodb)\n    - [PostgreSQL](#postgresql)\n    - [MariaDB](#mariadb)\n    - [MySQL](#mysql)\n    - [Redis](#redis)\n    - [Specify Storage Providers and Notifiers for each Database](#specify-storage-providers-and-notifiers-for-each-database)\n- [Storage Providers](#storage-providers)\n    - [S3](#s3)\n    - [Dropbox](#dropbox)\n- [Notifiers](#notifiers)\n    - [Discord](#discord)\n    - [Slack](#slack)\n    - [Telegram](#telegram)\n- [Rotation](#rotation)\n- [Cooldown](#cooldown)\n\n# Setup\n\nThis service can either be set up as a cron job (on UNIX systems), as a\nKubernetes CronJob, or scheduled in your favorite alternative scheduler.\n\n## Quick start\n\nRequires Python 3.9 or newer\n\n```sh\n# Install the CLI tool\npip install blackbox-cli\n\n# Create a configuration file\nblackbox --init\n\n# Run blackbox with a specific config file\nblackbox --config=/path/to/blackbox.yaml\n```\n\n### Setting up as a cron job\n\nAll you need to do to set it up as a cron job is clone this repo, create a\nconfig file (see below), and trigger `blackbox` to run automatically however\noften you want.\n\n```sh\ncrontab -e\n\n#run backup every hour\n0 */1 * * * blackbox --config path/to/blackbox.yml\n```\n\n### Setting it up as a Kubernetes CronJob\n\nTo set this up as a Kubernetes CronJob, you\'ll want three manifests and a\nsecret.\n\nBefore we start, you\'ll probably want to create a secret named `blackbox-secrets` where you expose\nenvironment variables containing stuff like passwords for your databases,\ncredentials for your storage, and webhooks as environment variables. We\'ll be\ninterpolating those into the config file.\n\nNext, we\'ll need a ConfigMap for the `blackbox.yaml` config file. See the\nConfiguration section below for more information on what to put inside this\nfile.\n\n```yaml\n# blackbox-configmap.yaml\napiVersion: v1\nkind: ConfigMap\nmetadata:\n  name: blackbox-config\ndata:\n  blackbox.yaml: |\n    databases:\n      mongodb:\n        main_mongodb:\n            connection_string: mongodb://{{ MONGO_INITDB_ROOT_USERNAME }}:{{ MONGO_INITDB_ROOT_PASSWORD }}@mongodb.default.svc.cluster.local:27017\n\n    storage:\n      s3:\n        main_s3:\n          bucket: blackbox\n          endpoint: my.s3.com\n          aws_access_key_id: {{ AWS_ACCESS_KEY_ID }}\n          aws_secret_access_key: {{ AWS_SECRET_ACCESS_KEY }}\n\n    notifiers:\n      discord:\n        main_discord:\n          webhook: {{ DISCORD_WEBHOOK }}\n\n    retention_days: 7\n```\n\nFinally, we need the CronJob itself. This one is configured to run once a day,\nat midnight.\n\n```yaml\n# cronjob.yaml\napiVersion: batch/v1\nkind: CronJob\nmetadata:\n  name: blackbox\nspec:\n  schedule: "@daily"\n  jobTemplate:\n    spec:\n      template:\n        spec:\n          containers:\n            - name: blackbox\n              image: lemonsaurus/blackbox\n              imagePullPolicy: Always\n              envFrom:\n                - secretRef:\n                    name: blackbox-secrets\n              # Tell blackbox where to find the config file.\n              env:\n              - name: BLACKBOX_CONFIG_PATH\n                value: "/blackbox/config_file/blackbox.yaml"\n              volumeMounts:\n                # Take care not to mount this in the root folder!\n                # That will replace everything in the root folder with\n                # the contents of this volume, which sucks.\n                - mountPath: /blackbox/config_file\n                  name: blackbox-config\n          volumes:\n            - name: blackbox-config\n              configMap:\n                name: blackbox-config\n          restartPolicy: OnFailure\n      backoffLimit: 3\n```\n\n# Configuration\n\n`blackbox` configuration is easy. You simply create a yaml\nfile, `blackbox.yaml`, which contains something like this:\n\nSee below for specific configuration information for each handler.\n\n```yaml\ndatabases:\n  postgres: # Database type \n    main_postgres: # Database identifier\n      # Configuration (see below for further information on specific databases)\n      username: username\n      password: password\n      host: host\n      port: port\n\n      # Optionally specify storage and notifiers to use\n      # You can specify them by type or identifier\n      # Use a string for a single specifier, a list for multiple specifiers\n      storage_providers:\n        - s3\n        - secondary_dropbox\n      notifiers: slack\n\n  redis:\n    main_redis:\n      password: password\n      host: host\n      port: port\n      # No specified storage and notifiers, so all storage and notifiers are used\n\nstorage:\n  s3: # Storage type\n    main_s3: # Storage identifier\n      bucket: bucket\n      endpoint: s3.endpoint.com\n    secondary_s3:\n      bucket: bucket\n      endpoint: s3.another_endpoint.com\n  dropbox:\n    main_dropbox:\n      access_token: XXXXXXXXXXX\n    secondary_dropbox:\n      access_token: XXXXXXXXXXX\n\nnotifiers:\n  discord: # Notifier type\n    main_discord: # Notifier identifier\n      webhook: https://discord.com/api/webhooks/797541821394714674/lzRM9DFggtfHZXGJTz3yE-MrYJ-4O-0AbdQg3uV2x4vFbu7HTHY2Njq8cx8oyMg0T3Wk\n  slack:\n    main_slack:\n      webhook: https://hooks.slack.com/services/XXXXXXXXXXX/XXXXXXXXXXX/XXXXXXXXXXXXXXXXXXX\n\nretention_days: 7\n```\n\nBlackbox will look for this file in the root folder by default, however you can\nprovide an alternative config file path by creating an environment variable\ncalled `BLACKBOX_CONFIG_PATH`, and set it to the absolute path of the file.\n\n```sh\nexport BLACKBOX_CONFIG_PATH=/var/my/favorite/fruit/blackbox.yaml\n```\n\nYou can also specify the location of this file when using the `blackbox` cli\ncommand.\n\n```sh\nblackbox --config=/path/to/blackbox.yaml\n```\n\n## Environment Variables\n\nThe `blackbox.yaml` will ✨ **magically interpolate** ✨ any environment\nvariables that exist in the environment where `blackbox` is running. This is\nvery useful if you want to keep your secrets in environment variables, instead\nof keeping them in the config file in plaintext.\n\n#### Example\n\nImagine your current config looks like this, but you want to move the username\nand password into environment variables.\n\n```yaml\ndatabases:\n  postgres:\n    main_postgres:\n      username: lemonsaurus\n      password: security-is-overrated\n      host: localhost\n      port: 5432\n```\n\nSo we\'ll create two environment variables like these:\n\n```sh\nexport POSTGRES_USERNAME=lemonsaurus\nexport POSTGRES_PASSWORD=security-is-overrated\n```\n\nAnd now we can make use of these environment variables by using double curly\nbrackets, like this:\n\n```yaml\ndatabases:\n  postgres:\n    main_postgres:\n      username: { { POSTGRES_USERNAME } }\n      password: { { POSTGRES_PASSWORD } }\n      host: localhost\n      port: 5432\n```\n\n## Databases\n\nRight now, this app supports **MongoDB**, **PostgreSQL 7.0 or higher**, **MariaDB**, **Redis** and **local storage archiving**. If\nyou need support for an additional database, consider opening a pull request to\nadd a new database handler.\n\nTo configure databases, add a section with this format:\n\n```yaml\ndatabases:\n  database_type:\n    # More than one of each database type can be configured\n    identifier_1:\n      field: value\n    identifier_2:\n      field: value\n  database_type:\n    ...\n```\n\nSee below for the specific database types available and fields required.\nIdentifiers can be any string of your choosing.\n\n### MongoDB\n\n- **Database Type**: `mongodb`\n- **Required fields**: `connection_string`\n- The `connection_string` field is in the\n  format `mongodb://username:password@host:port`\n- To restore from the backup,\n  use `mongorestore --gzip --archive=/path/to/backup.archive`\n\n```yaml\n  mongodb:\n    main_mongo:\n      connection_string: "mongodb://blackbox:blackbox@mongo:27017"\n```\n\n### PostgreSQL\n\n- **Database Type**: `postgres`\n- **Required fields**: `username`, `password`, `host`, `port`\n- To restore from the backup, use `psql -f /path/to/backup.sql`\n\n```yaml\n  postgres:\n    main_postgres:\n      username: blackbox\n      password: blackbox\n      host: postgres\n      port: "5432"\n```\n\n### MariaDB\n\n- **Database Type**: `mariadb`\n- **Required fields**: `username`, `password`, `host`, `port`\n- To restore from the backup, use `mysql -u <user> -p < db_backup.sql`\n\n```yaml\n  mariadb:\n    main_mariadb:\n      username: root\n      password: example\n      host: maria\n      port: "3306"\n```\n\n### MySQL\n\n- **Database Type**: `mysql`\n- **Required fields**: `username`, `password`, `host`, `port`\n- To restore from the backup, use `mysql -u <user> -p < db_backup.sql`\n\n```yaml\n  mysql:\n    main_mysql:\n      username: root\n      password: example\n      host: mysql\n      port: "3306"\n```\n\n### Redis\n\n- **Database Type**: `redis`\n- **Required fields**: `password`, `host`, `port`\n\n```yaml\n  redis:\n    main_redis:\n      password: blackbox\n      host: redis\n      port: "6379"\n```\n\n### Local storage\n\n- **Database type**: `localstorage`\n- **Required field**: `path`\n- **Optional field**: `compression_level`\n- The compression level must be an integer between 0 and 9.\n- The archive will contain the full structure, starting from the root folder.\n\n```yaml\n  localstorage:\n    main_localstorage:\n      path: /path/to/folder\n      compression_level: 7\n```\n\n#### To restore from the backup\n\n- Stop Redis server.\n- Turn off `appendonly` mode in Redis configuration (set to `no`).\n- Copy backup file to Redis working directory (`dir` in configuration) with\n  name that is defined in configuration key `dbfilename`.\n- Set backup permissions.\n\n```\nsudo chown redis:redis <path-to-redis-dump-file>\nsudo chmod 660 <path-to-redis-dump-file>\n```\n\n- Start Redis server.\n\nIf you want to re-enable `appendonly`:\n\n- Login with `redis-cli`.\n- Run `BGREWRITEAOF`.\n- Exit from Redis CLI (with `exit`).\n- Stop Redis server.\n- Set `appendonly` to `yes` in Redis configuration.\n- Start Redis server.\n\n### Specify Storage providers and Notifiers for each Database\n\nTo specify specific storage providers or notifiers for databases, add the\nfields `storage_providers` and `notifiers` under each database entry. The entry\ncan be a list or a string.\n\n```yaml\ndatabases:\n  postgres: # Database type \n    main_postgres: # Database identifier\n      username: username\n      password: password\n      host: host\n      port: port\n\n      storage_providers:\n        - s3\n        - secondary_dropbox\n      notifiers: slack\n```\n\nThe above example will backup `main_postgres` to every `s3` storage provider\nconfigured, as well as the storage provider with the\nidentifier `secondary_dropbox`. Then, only the `slack` notifier gets notified.\n\nThese fields are optional. If not given, all storage providers and all\nnotifiers will be used.\n\n## Storage providers\n\n**Blackbox** can work with different storage providers to save your logs and\nbackups - usually so that you can automatically store them in the cloud. Right\nnow we support **S3** and **Dropbox**.\n\nTo configure storage providers, add a section with this format:\n\n```yaml\nstorage:\n  storage_type:\n    # More than one of each storage provider type can be configured\n    identifier_1:\n      field: value\n    identifier_2:\n      field: value\n  storage_type:\n    ...\n```\n\n### S3\n\nWe support any S3 object storage bucket, whether it\'s from **AWS**, **Linode**\n, **DigitalOcean**, **Scaleway**, or another S3-compatible object storage\nprovider.\n\n**Blackbox** will respect the `retention_days` configuration setting and delete\nolder files from the S3 storage. Please note that if you have a bucket\nexpiration policy on your storage, **blackbox** will not do anything to disable\nit. So, for example, if your bucket expiration policy is 12 hours and blackbox\nis set to 7 `retention_days`, then your backups are all gonna be deleted after\n12 hours unless you disable your policy.\n\n#### S3 configuration\n\n- **Storage Type**: `s3`\n- **Required fields**: `bucket`, `endpoint`\n- **Optional fields**: `aws_access_key_id`, `aws_secret_access_key`\n- The `endpoint` field can look something like\n  this: `s3.eu-west-1.amazonaws.com`\n\n#### Credentials\n\nTo upload stuff to S3, you\'ll need credentials. Your **AWS credentials** can be\nprovided in several ways. This is the order in which blackbox looks for them:\n\n- First, we look for the optional fields in the s3 configuration,\n  called `aws_access_key_id` and `aws_secret_access_key`.\n- If these are not found, we\'ll check if the `AWS_ACCESS_KEY_ID`\n  and `AWS_SECRET_ACCESS_KEY` environment variables are declared in the local\n  environment where Blackbox is running.\n- If we can\'t find these, we\'ll look for an `.aws/config` file in the local\n  environment.\n- NOTE: If the bucket is public, no credentials are necessary.\n\n### Dropbox\n\n- **Storage Type**: `dropbox`\n- **Required fields**: `access_token`\n- **Optional fields**: `upload_directory`\n\nThe Dropbox storage handler needs a user access token in order to work. To get\none, do the following:\n\n- Create a Dropbox account (if you don\'t already have one).\n- Go to https://dropbox.com/developers\n- Create a new application with App Folder access. **Do not give it full\n  access**, as this may have dangerous, destructive consequences if configured\n  incorrectly.\n\nYou can also define a custom location (root is App Folder) using the\n`upload_directory` optional parameter. This **should** begin with slash and \n**must** end with slash. Default is root.\n\n## Notifiers\n\n`blackbox` also implements different _notifiers_, which is how it reports the\nresult of one of its jobs to you. Right now we only support **Discord** and **Slack**\nand **Telegram**, but if you need a specific notifier, feel free to open an issue.\n\nTo configure notifiers, add a section with this format:\n\n```yaml\nnotifiers:\n  notifier_type:\n    # More than one of each notifier type can be configured\n    identifier_1:\n      field: value\n    identifier_2:\n      field: value\n  notifier_type:\n    ...\n```\n\n### Discord\n\n- **Notifier Type**: `discord`\n- **Required fields**: `webhook`\n- The `webhook` field usually looks\n  like `https://discord.com/api/webhooks/797541821394714674/lzRM9DFggtfHZXGJTz3yE-MrYJ-4O-0AbdQg3uV2x4vFbu7HTHY2Njq8cx8oyMg0T3Wk`\n- We also support `ptb.discord.com` and `canary.discord.com` webhooks.\n\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_discord.png)\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_discord_2.png)\n\n### Slack\n\n- **Notifier Type**: `slack`\n- **Required fields**: `webhook`\n- The `webhook` field usually looks\n  like `https://hooks.slack.com/services/XXXXXXXXXXX/XXXXXXXXXXX/XXXXXXXXXXXXXXXXXXX`\n\nSlack notifiers have 2 styles: legacy attachment (default) and modern Block Kit\nversion. To enable Block Kit version, set the optional field `use_block_kit` to\nanything.\n\nDefault:\n\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_slack_default_success.png)\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_slack_default_fail.png)\n\nModern:\n\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_slack_modern_success.png)\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_slack_modern_fail.png)\n\n\n### Telegram\n\n- **Notifier Type**: `telegram`\n- **Required fields**: `token`, `chat_id`\n- YAML will look like this:\n```notifiers:\n  telegram:\n    telegram_1:\n      token: {{ TELEGRAM_TOKEN }}\n      chat_id: {{ TELEGRAM_CHAT_ID }}\n```\n- You can create a bot and get a bot token using the `BotFather` account in Telegram. Follow [these instructions](https://core.telegram.org/bots#6-botfather).\n- You can find your `chat_id` by using the `userinfobot` account in Telegram. Just `/start` the bot.\n- Do not forget to `/start` your own bot to grant sending permissions.\n\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_telegram_success.png)\n![blackbox](https://github.com/lemonsaurus/blackbox/raw/main/img/blackbox_telegram_fail.png)\n\n\n## Rotation\n\nBy default, `blackbox` will automatically remove all backup files older than 7\ndays in the folder you configure for your storage provider. To determine if\nsomething is a backup file or not, it will use a regex pattern that corresponds\nwith the default file it saves, for\nexample `blackbox-postgres-backup-11-12-2020.sql`.\n\nYou can configure the number of days before rotating by altering\nthe `retention_days` parameter in `blackbox.yaml`.\n\n\n## Cooldown\n\nBy default, `blackbox` will send all notification at every backup attempt. \nYou can specify a `cooldown` period in `blackbox.yaml` during which all notifications will be muted.\nThis option will not mute failed backups.\n\n### Example usage\n\n```yaml\ncooldown: 120s\n```\n```yaml\ncooldown: 3 hours\n```\n```yaml\ncooldown: 2 days 4 hours\n```\n```yaml\ncooldown: 4h 32M 16s\n```\n',
     'author': 'Leon Sandøy',
     'author_email': 'leon.sandoy@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lemonsaurus/blackbox',
```

### Comparing `blackbox_cli-2.3.2/PKG-INFO` & `blackbox_cli-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackbox-cli
-Version: 2.3.2
+Version: 2.4.0
 Summary: Tool for automatic backups of databases
 Home-page: https://github.com/lemonsaurus/blackbox
 License: MIT
 Author: Leon Sandøy
 Author-email: leon.sandoy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Archiving :: Backup
 Requires-Dist: boto3 (>=1.16.51,<2.0.0)
-Requires-Dist: click (>=7.1.2,<8.0.0)
+Requires-Dist: click (>=7.1.2,<9.0.0)
 Requires-Dist: dropbox (>=11.0.0,<12.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: pytelegrambotapi (>=3.7.7,<4.0.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: single-source (>=0.2.0,<0.3.0)
```

