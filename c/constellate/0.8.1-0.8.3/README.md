# Comparing `tmp/constellate-0.8.1-py2.py3-none-any.whl.zip` & `tmp/constellate-0.8.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,172 +1,181 @@
-Zip file size: 115082 bytes, number of entries: 170
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/__init__.py
--rw-rw-rw-  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/py.typed
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/cli/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/cli/argument/__init__.py
--rw-r--r--  2.0 unx     1410 b- defN 23-Sep-14 06:48 constellate/cli/argument/unparse.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/compression/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/compression/zip/__init__.py
--rw-r--r--  2.0 unx     2575 b- defN 23-Sep-14 06:48 constellate/compression/zip/zip.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/concurrency/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/concurrency/asyncio/__init__.py
--rw-r--r--  2.0 unx     3009 b- defN 23-Sep-14 06:48 constellate/concurrency/asyncio/tasks.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/concurrency/pebble/__init__.py
--rw-r--r--  2.0 unx     2695 b- defN 23-Sep-14 06:48 constellate/concurrency/pebble/pool_cleanup.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/concurrency/simple/__init__.py
--rw-r--r--  2.0 unx     4056 b- defN 23-Sep-14 06:48 constellate/concurrency/simple/simple.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/concurrency/std/__init__.py
--rw-r--r--  2.0 unx      591 b- defN 23-Sep-14 06:48 constellate/concurrency/std/pool.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/constant/__init__.py
--rw-r--r--  2.0 unx      250 b- defN 23-Sep-14 06:48 constellate/constant/concurrency.py
--rw-r--r--  2.0 unx       22 b- defN 23-Sep-14 06:48 constellate/constant/debug.py
--rw-r--r--  2.0 unx      102 b- defN 23-Sep-14 06:48 constellate/constant/platform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/container/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/container/orchestration/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/container/orchestration/k8s/__init__.py
--rw-r--r--  2.0 unx      447 b- defN 23-Sep-14 06:48 constellate/container/orchestration/k8s/probe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/cryptography/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/cryptography/digest/__init__.py
--rw-r--r--  2.0 unx     1809 b- defN 23-Sep-14 06:48 constellate/cryptography/digest/hexadecimal.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/common/__init__.py
--rw-r--r--  2.0 unx      121 b- defN 23-Sep-14 06:48 constellate/database/common/databasetype.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/migration/__init__.py
--rw-r--r--  2.0 unx      697 b- defN 23-Sep-14 06:48 constellate/database/migration/constant.py
--rw-r--r--  2.0 unx     2220 b- defN 23-Sep-14 06:48 constellate/database/migration/metadata.py
--rw-r--r--  2.0 unx     6720 b- defN 23-Sep-14 06:48 constellate/database/migration/migrate.py
--rw-r--r--  2.0 unx     3429 b- defN 23-Sep-14 06:48 constellate/database/migration/migrationcontext.py
--rw-r--r--  2.0 unx     9565 b- defN 23-Sep-14 06:48 constellate/database/migration/migrationstep.py
--rw-r--r--  2.0 unx      372 b- defN 23-Sep-14 06:48 constellate/database/migration/tablecontext.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/migration/standard/__init__.py
--rw-r--r--  2.0 unx      445 b- defN 23-Sep-14 06:48 constellate/database/migration/standard/base.py
--rw-r--r--  2.0 unx    22344 b- defN 23-Sep-14 06:48 constellate/database/migration/standard/migrate.py
--rw-r--r--  2.0 unx     2492 b- defN 23-Sep-14 06:48 constellate/database/migration/standard/table.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sparql/__init__.py
--rw-r--r--  2.0 unx      606 b- defN 23-Sep-14 06:48 constellate/database/sparql/query.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sparql/sparqlburger/__init__.py
--rw-r--r--  2.0 unx      553 b- defN 23-Sep-14 06:48 constellate/database/sparql/sparqlburger/triple.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/__init__.py
--rw-r--r--  2.0 unx      180 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/relationshiptype.py
--rw-r--r--  2.0 unx    32367 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sqlalchemy.py
--rw-r--r--  2.0 unx      810 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sqlalchemydbconfig.py
--rw-r--r--  2.0 unx     1477 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
--rw-r--r--  2.0 unx     1004 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sqlalchemyengineconfig.py
--rw-r--r--  2.0 unx      215 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
--rw-r--r--  2.0 unx    12933 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sqlalchemypostgresql.py
--rw-r--r--  2.0 unx     9931 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sqlalchemysqlite3.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/crud/__init__.py
--rw-r--r--  2.0 unx     6311 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/crud/cru.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/exception/__init__.py
--rw-r--r--  2.0 unx       46 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/exception/migrationexception.py
--rw-r--r--  2.0 unx       42 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/exception/vacumexception.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/execution/__init__.py
--rw-r--r--  2.0 unx     7580 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/execution/execute.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/schema/__init__.py
--rw-r--r--  2.0 unx     1462 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/schema/create.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/schema/drop.py
--rw-r--r--  2.0 unx     1752 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/schema/setsearchpath.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/table/__init__.py
--rw-r--r--  2.0 unx     2344 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/table/drop.py
--rw-r--r--  2.0 unx     3576 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/table/presence.py
--rw-r--r--  2.0 unx     1105 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/expression/table/truncate.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/session/__init__.py
--rw-r--r--  2.0 unx     6196 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/session/multienginesession.py
--rw-r--r--  2.0 unx     3778 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/session/syncmultienginesession.py
--rw-r--r--  2.0 unx     3097 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/session/binder/__init__.py
--rw-r--r--  2.0 unx     1813 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/session/binder/binderresolver.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sharding/__init__.py
--rw-r--r--  2.0 unx     7054 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sharding/sharder.py
--rw-r--r--  2.0 unx      529 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sharding/shardoption.py
--rw-r--r--  2.0 unx     2468 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sharding/simplesession.py
--rw-r--r--  2.0 unx     2103 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/sharding/unittoshardmixin.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/typedecorator/__init__.py
--rw-r--r--  2.0 unx      756 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/typedecorator/enuminteger.py
--rw-r--r--  2.0 unx      755 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/typedecorator/enumstring.py
--rw-r--r--  2.0 unx     2097 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/typedecorator/enumvalue.py
--rw-r--r--  2.0 unx      576 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/typedecorator/timestamptz.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/types/__init__.py
--rw-r--r--  2.0 unx    16084 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/types/composite.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/utils/__init__.py
--rw-r--r--  2.0 unx      479 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/utils/sessioncommit.py
--rw-r--r--  2.0 unx     1681 b- defN 23-Sep-14 06:48 constellate/database/sqlalchemy/utils/sql_query.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/database/sqlite3/__init__.py
--rw-r--r--  2.0 unx     1932 b- defN 23-Sep-14 06:48 constellate/database/sqlite3/sqlite3.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/datatype/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/datatype/dictionary/__init__.py
--rw-r--r--  2.0 unx      383 b- defN 23-Sep-14 06:48 constellate/datatype/dictionary/pop.py
--rw-r--r--  2.0 unx      663 b- defN 23-Sep-14 06:48 constellate/datatype/dictionary/update.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/datatype/enum/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 23-Sep-14 06:48 constellate/datatype/enum/enum.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/datetime/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/datetime/timeinterval/__init__.py
--rw-r--r--  2.0 unx    11006 b- defN 23-Sep-14 06:48 constellate/datetime/timeinterval/timeinterval.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/debug/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/debug/packages/__init__.py
--rw-r--r--  2.0 unx       88 b- defN 23-Sep-14 06:48 constellate/debug/packages/package.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/debugger/__init__.py
--rw-r--r--  2.0 unx     1374 b- defN 23-Sep-14 06:48 constellate/debugger/debugger.py
--rw-r--r--  2.0 unx      737 b- defN 23-Sep-14 06:48 constellate/debugger/simple.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/logger/__init__.py
--rw-r--r--  2.0 unx    18698 b- defN 23-Sep-14 06:48 constellate/logger/log.py
--rw-r--r--  2.0 unx     3980 b- defN 23-Sep-14 06:48 constellate/logger/loggers.py
--rw-r--r--  2.0 unx      652 b- defN 23-Sep-14 06:48 constellate/logger/logmode.py
--rw-r--r--  2.0 unx     3050 b- defN 23-Sep-14 06:48 constellate/logger/simple.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/logger/handler/__init__.py
--rw-r--r--  2.0 unx      562 b- defN 23-Sep-14 06:48 constellate/logger/handler/forwarderhandler.py
--rw-r--r--  2.0 unx      569 b- defN 23-Sep-14 06:48 constellate/logger/handler/stringhandler.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/network/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/network/download/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/network/url/__init__.py
--rw-r--r--  2.0 unx      248 b- defN 23-Sep-14 06:48 constellate/network/url/unshortener.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/package/__init__.py
--rw-r--r--  2.0 unx      173 b- defN 23-Sep-14 06:48 constellate/package/package.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/pretty/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/pretty/log/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 23-Sep-14 06:48 constellate/pretty/log/line.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/progression/__init__.py
--rw-r--r--  2.0 unx     1013 b- defN 23-Sep-14 06:48 constellate/progression/progres.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/project/__init__.py
--rw-r--r--  2.0 unx      202 b- defN 23-Sep-14 06:48 constellate/project/version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/resource/__init__.py
--rw-r--r--  2.0 unx     2206 b- defN 23-Sep-14 06:48 constellate/resource/resource.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/storage/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/anyfs/__init__.py
--rw-r--r--  2.0 unx      127 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/anyfs/availability.py
--rw-r--r--  2.0 unx     3808 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/anyfs/path.py
--rw-r--r--  2.0 unx      264 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/anyfs/size.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/tmpfs/__init__.py
--rw-r--r--  2.0 unx     6635 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/tmpfs/memory_tempfile.py
--rw-r--r--  2.0 unx     2631 b- defN 23-Sep-14 06:48 constellate/storage/filesystem/tmpfs/rambacked.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/testing/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/testing/mock/__init__.py
--rw-r--r--  2.0 unx      374 b- defN 23-Sep-14 06:48 constellate/testing/mock/argv.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/__init__.py
--rw-r--r--  2.0 unx      596 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/accessor/__init__.py
--rw-r--r--  2.0 unx     3173 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/accessor/attribute_accessor.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/extra/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/extra/sanitize/__init__.py
--rw-r--r--  2.0 unx    11089 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/extra/sanitize/sanitize.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/io/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/io/sql/__init__.py
--rw-r--r--  2.0 unx     2570 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/io/sql/sqlalchemy.py
--rw-r--r--  2.0 unx      565 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py
--rw-r--r--  2.0 unx     1127 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/validation/__init__.py
--rw-r--r--  2.0 unx      624 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/validation/pandera.py
--rw-r--r--  2.0 unx     6050 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandas/validation/validation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandera/__init__.py
--rw-r--r--  2.0 unx     1660 b- defN 23-Sep-14 06:48 constellate/thirdparty/pandera/inspector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/virtualization/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/virtualization/common/__init__.py
--rw-r--r--  2.0 unx      214 b- defN 23-Sep-14 06:48 constellate/virtualization/common/common.py
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 06:48 constellate/virtualization/docker/__init__.py
--rw-rw-rw-  2.0 unx       47 b- defN 23-Sep-14 06:48 constellate-0.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3470 b- defN 23-Sep-14 06:48 constellate-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Sep-14 06:48 constellate-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Sep-14 06:48 constellate-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    16887 b- defN 23-Sep-14 06:48 constellate-0.8.1.dist-info/RECORD
-170 files, 310631 bytes uncompressed, 87116 bytes compressed:  72.0%
+Zip file size: 118821 bytes, number of entries: 179
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-04 15:56 constellate/py.typed
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/cli/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/cli/argument/__init__.py
+-rw-r--r--  2.0 unx     1410 b- defN 24-May-04 15:56 constellate/cli/argument/unparse.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/compression/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/compression/zip/__init__.py
+-rw-r--r--  2.0 unx     2575 b- defN 24-May-04 15:56 constellate/compression/zip/zip.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/concurrency/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/concurrency/asyncio/__init__.py
+-rw-r--r--  2.0 unx     3009 b- defN 24-May-04 15:56 constellate/concurrency/asyncio/tasks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/concurrency/pebble/__init__.py
+-rw-r--r--  2.0 unx     2687 b- defN 24-May-04 15:56 constellate/concurrency/pebble/pool_cleanup.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/concurrency/simple/__init__.py
+-rw-r--r--  2.0 unx     4056 b- defN 24-May-04 15:56 constellate/concurrency/simple/simple.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/concurrency/std/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 24-May-04 15:56 constellate/concurrency/std/pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/constant/__init__.py
+-rw-r--r--  2.0 unx      250 b- defN 24-May-04 15:56 constellate/constant/concurrency.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-04 15:56 constellate/constant/debug.py
+-rw-r--r--  2.0 unx      102 b- defN 24-May-04 15:56 constellate/constant/platform.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/container/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/container/orchestration/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/container/orchestration/k8s/__init__.py
+-rw-r--r--  2.0 unx      447 b- defN 24-May-04 15:56 constellate/container/orchestration/k8s/probe.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/cryptography/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/cryptography/digest/__init__.py
+-rw-r--r--  2.0 unx     1793 b- defN 24-May-04 15:56 constellate/cryptography/digest/hexadecimal.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/common/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 24-May-04 15:56 constellate/database/common/databasetype.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/migration/__init__.py
+-rw-r--r--  2.0 unx      697 b- defN 24-May-04 15:56 constellate/database/migration/constant.py
+-rw-r--r--  2.0 unx     2220 b- defN 24-May-04 15:56 constellate/database/migration/metadata.py
+-rw-r--r--  2.0 unx     6720 b- defN 24-May-04 15:56 constellate/database/migration/migrate.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-04 15:56 constellate/database/migration/migrationcontext.py
+-rw-r--r--  2.0 unx     9621 b- defN 24-May-04 15:56 constellate/database/migration/migrationstep.py
+-rw-r--r--  2.0 unx      372 b- defN 24-May-04 15:56 constellate/database/migration/tablecontext.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/migration/standard/__init__.py
+-rw-r--r--  2.0 unx      445 b- defN 24-May-04 15:56 constellate/database/migration/standard/base.py
+-rw-r--r--  2.0 unx    22344 b- defN 24-May-04 15:56 constellate/database/migration/standard/migrate.py
+-rw-r--r--  2.0 unx     2492 b- defN 24-May-04 15:56 constellate/database/migration/standard/table.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sparql/__init__.py
+-rw-r--r--  2.0 unx      606 b- defN 24-May-04 15:56 constellate/database/sparql/query.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sparql/sparqlburger/__init__.py
+-rw-r--r--  2.0 unx      553 b- defN 24-May-04 15:56 constellate/database/sparql/sparqlburger/triple.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/__init__.py
+-rw-r--r--  2.0 unx      180 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/relationshiptype.py
+-rw-r--r--  2.0 unx    32367 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sqlalchemy.py
+-rw-r--r--  2.0 unx      810 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sqlalchemydbconfig.py
+-rw-r--r--  2.0 unx     1477 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
+-rw-r--r--  2.0 unx     1004 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sqlalchemyengineconfig.py
+-rw-r--r--  2.0 unx      215 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
+-rw-r--r--  2.0 unx    13143 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sqlalchemypostgresql.py
+-rw-r--r--  2.0 unx     9931 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sqlalchemysqlite3.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/crud/__init__.py
+-rw-r--r--  2.0 unx     6311 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/crud/cru.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/exception/__init__.py
+-rw-r--r--  2.0 unx       46 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/exception/migrationexception.py
+-rw-r--r--  2.0 unx       42 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/exception/vacumexception.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/execution/__init__.py
+-rw-r--r--  2.0 unx     7580 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/execution/execute.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/schema/__init__.py
+-rw-r--r--  2.0 unx     1510 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/schema/create.py
+-rw-r--r--  2.0 unx     1231 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/schema/drop.py
+-rw-r--r--  2.0 unx     1752 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/schema/setsearchpath.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/table/__init__.py
+-rw-r--r--  2.0 unx     2344 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/table/drop.py
+-rw-r--r--  2.0 unx     1641 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/table/lock.py
+-rw-r--r--  2.0 unx     3576 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/table/presence.py
+-rw-r--r--  2.0 unx     1105 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/expression/table/truncate.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/session/__init__.py
+-rw-r--r--  2.0 unx     6196 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/session/multienginesession.py
+-rw-r--r--  2.0 unx     3778 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/session/syncmultienginesession.py
+-rw-r--r--  2.0 unx     3097 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/session/binder/__init__.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/session/binder/binderresolver.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sharding/__init__.py
+-rw-r--r--  2.0 unx     7054 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sharding/sharder.py
+-rw-r--r--  2.0 unx      529 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sharding/shardoption.py
+-rw-r--r--  2.0 unx     2468 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sharding/simplesession.py
+-rw-r--r--  2.0 unx     2103 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/sharding/unittoshardmixin.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/typedecorator/__init__.py
+-rw-r--r--  2.0 unx      756 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/typedecorator/enuminteger.py
+-rw-r--r--  2.0 unx      755 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/typedecorator/enumstring.py
+-rw-r--r--  2.0 unx     2097 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/typedecorator/enumvalue.py
+-rw-r--r--  2.0 unx      576 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/typedecorator/timestamptz.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/types/__init__.py
+-rw-r--r--  2.0 unx    16084 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/types/composite.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/utils/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/utils/sessioncommit.py
+-rw-r--r--  2.0 unx     1681 b- defN 24-May-04 15:56 constellate/database/sqlalchemy/utils/sql_query.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/database/sqlite3/__init__.py
+-rw-r--r--  2.0 unx     1932 b- defN 24-May-04 15:56 constellate/database/sqlite3/sqlite3.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/datatype/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/datatype/dictionary/__init__.py
+-rw-r--r--  2.0 unx      383 b- defN 24-May-04 15:56 constellate/datatype/dictionary/pop.py
+-rw-r--r--  2.0 unx      663 b- defN 24-May-04 15:56 constellate/datatype/dictionary/update.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/datatype/enum/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 24-May-04 15:56 constellate/datatype/enum/enum.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/datetime/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/datetime/timeinterval/__init__.py
+-rw-r--r--  2.0 unx    11006 b- defN 24-May-04 15:56 constellate/datetime/timeinterval/timeinterval.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/debug/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/debug/packages/__init__.py
+-rw-r--r--  2.0 unx       88 b- defN 24-May-04 15:56 constellate/debug/packages/package.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/debugger/__init__.py
+-rw-r--r--  2.0 unx     1374 b- defN 24-May-04 15:56 constellate/debugger/debugger.py
+-rw-r--r--  2.0 unx      737 b- defN 24-May-04 15:56 constellate/debugger/simple.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/logger/__init__.py
+-rw-r--r--  2.0 unx    20086 b- defN 24-May-04 15:56 constellate/logger/log.py
+-rw-r--r--  2.0 unx     3980 b- defN 24-May-04 15:56 constellate/logger/loggers.py
+-rw-r--r--  2.0 unx      652 b- defN 24-May-04 15:56 constellate/logger/logmode.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-May-04 15:56 constellate/logger/simple.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/logger/formatter/__init__.py
+-rw-r--r--  2.0 unx      785 b- defN 24-May-04 15:56 constellate/logger/formatter/formatterfactory.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/logger/handler/__init__.py
+-rw-r--r--  2.0 unx      562 b- defN 24-May-04 15:56 constellate/logger/handler/forwarderhandler.py
+-rw-r--r--  2.0 unx      569 b- defN 24-May-04 15:56 constellate/logger/handler/stringhandler.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/network/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/network/download/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/network/url/__init__.py
+-rw-r--r--  2.0 unx      248 b- defN 24-May-04 15:56 constellate/network/url/unshortener.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/package/__init__.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-04 15:56 constellate/package/package.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/pretty/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/pretty/log/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 24-May-04 15:56 constellate/pretty/log/line.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/progression/__init__.py
+-rw-r--r--  2.0 unx     1013 b- defN 24-May-04 15:56 constellate/progression/progres.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/project/__init__.py
+-rw-r--r--  2.0 unx      202 b- defN 24-May-04 15:56 constellate/project/version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/resource/__init__.py
+-rw-r--r--  2.0 unx     2206 b- defN 24-May-04 15:56 constellate/resource/resource.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/storage/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/storage/filesystem/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/storage/filesystem/anyfs/__init__.py
+-rw-r--r--  2.0 unx      127 b- defN 24-May-04 15:56 constellate/storage/filesystem/anyfs/availability.py
+-rw-r--r--  2.0 unx     3808 b- defN 24-May-04 15:56 constellate/storage/filesystem/anyfs/path.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-04 15:56 constellate/storage/filesystem/anyfs/size.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/storage/filesystem/tmpfs/__init__.py
+-rw-r--r--  2.0 unx     6635 b- defN 24-May-04 15:56 constellate/storage/filesystem/tmpfs/memory_tempfile.py
+-rw-r--r--  2.0 unx     2631 b- defN 24-May-04 15:56 constellate/storage/filesystem/tmpfs/rambacked.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/testing/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/testing/mock/__init__.py
+-rw-r--r--  2.0 unx      374 b- defN 24-May-04 15:56 constellate/testing/mock/argv.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/numba/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/numba/progress/__init__.py
+-rw-r--r--  2.0 unx     1074 b- defN 24-May-04 15:56 constellate/thirdparty/numba/progress/progress.py
+-rw-r--r--  2.0 unx      596 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/accessor/__init__.py
+-rw-r--r--  2.0 unx     3173 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/accessor/attribute_accessor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/extra/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/extra/sanitize/__init__.py
+-rw-r--r--  2.0 unx    11089 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/extra/sanitize/sanitize.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/io/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/io/sql/__init__.py
+-rw-r--r--  2.0 unx     2570 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/io/sql/sqlalchemy.py
+-rw-r--r--  2.0 unx      565 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py
+-rw-r--r--  2.0 unx     1127 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/operation/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/operation/introspection/__init__.py
+-rw-r--r--  2.0 unx      336 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/operation/introspection/introspection.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/validation/__init__.py
+-rw-r--r--  2.0 unx      624 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/validation/pandera.py
+-rw-r--r--  2.0 unx     6050 b- defN 24-May-04 15:56 constellate/thirdparty/pandas/validation/validation.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/thirdparty/pandera/__init__.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-04 15:56 constellate/thirdparty/pandera/inspector.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/virtualization/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/virtualization/common/__init__.py
+-rw-r--r--  2.0 unx      214 b- defN 24-May-04 15:56 constellate/virtualization/common/common.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-04 15:56 constellate/virtualization/docker/__init__.py
+-rw-rw-rw-  2.0 unx       47 b- defN 24-May-04 15:57 constellate-0.8.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3470 b- defN 24-May-04 15:57 constellate-0.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-04 15:57 constellate-0.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-04 15:57 constellate-0.8.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17851 b- defN 24-May-04 15:57 constellate-0.8.3.dist-info/RECORD
+179 files, 317109 bytes uncompressed, 89235 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -201,14 +201,17 @@
 
 Filename: constellate/database/sqlalchemy/expression/table/__init__.py
 Comment: 
 
 Filename: constellate/database/sqlalchemy/expression/table/drop.py
 Comment: 
 
+Filename: constellate/database/sqlalchemy/expression/table/lock.py
+Comment: 
+
 Filename: constellate/database/sqlalchemy/expression/table/presence.py
 Comment: 
 
 Filename: constellate/database/sqlalchemy/expression/table/truncate.py
 Comment: 
 
 Filename: constellate/database/sqlalchemy/session/__init__.py
@@ -336,14 +339,20 @@
 
 Filename: constellate/logger/logmode.py
 Comment: 
 
 Filename: constellate/logger/simple.py
 Comment: 
 
+Filename: constellate/logger/formatter/__init__.py
+Comment: 
+
+Filename: constellate/logger/formatter/formatterfactory.py
+Comment: 
+
 Filename: constellate/logger/handler/__init__.py
 Comment: 
 
 Filename: constellate/logger/handler/forwarderhandler.py
 Comment: 
 
 Filename: constellate/logger/handler/stringhandler.py
@@ -429,14 +438,23 @@
 
 Filename: constellate/testing/mock/argv.py
 Comment: 
 
 Filename: constellate/thirdparty/__init__.py
 Comment: 
 
+Filename: constellate/thirdparty/numba/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/numba/progress/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/numba/progress/progress.py
+Comment: 
+
 Filename: constellate/thirdparty/pandas/__init__.py
 Comment: 
 
 Filename: constellate/thirdparty/pandas/accessor/__init__.py
 Comment: 
 
 Filename: constellate/thirdparty/pandas/accessor/attribute_accessor.py
@@ -462,14 +480,23 @@
 
 Filename: constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py
 Comment: 
 
 Filename: constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py
 Comment: 
 
+Filename: constellate/thirdparty/pandas/operation/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/operation/introspection/__init__.py
+Comment: 
+
+Filename: constellate/thirdparty/pandas/operation/introspection/introspection.py
+Comment: 
+
 Filename: constellate/thirdparty/pandas/validation/__init__.py
 Comment: 
 
 Filename: constellate/thirdparty/pandas/validation/pandera.py
 Comment: 
 
 Filename: constellate/thirdparty/pandas/validation/validation.py
@@ -489,23 +516,23 @@
 
 Filename: constellate/virtualization/common/common.py
 Comment: 
 
 Filename: constellate/virtualization/docker/__init__.py
 Comment: 
 
-Filename: constellate-0.8.1.dist-info/LICENSE
+Filename: constellate-0.8.3.dist-info/LICENSE
 Comment: 
 
-Filename: constellate-0.8.1.dist-info/METADATA
+Filename: constellate-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: constellate-0.8.1.dist-info/WHEEL
+Filename: constellate-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: constellate-0.8.1.dist-info/top_level.txt
+Filename: constellate-0.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: constellate-0.8.1.dist-info/RECORD
+Filename: constellate-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## constellate/concurrency/pebble/pool_cleanup.py

```diff
@@ -7,16 +7,15 @@
 
 """
 Clean up pebble process pool on signals
 """
 
 
 class PostPebblePoolCleanup(Protocol):
-    def __call__(self, forced_shutdown: bool = False) -> None:
-        ...
+    def __call__(self, forced_shutdown: bool = False) -> None: ...
 
 
 def _pebble_cleanup_pool(
     force_shutdown: bool = False,
     pool: pebble.ProcessPool = None,
     futures: List[pebble.ProcessFuture] = [],
     post_cleanup: PostPebblePoolCleanup = None,
```

## constellate/cryptography/digest/hexadecimal.py

```diff
@@ -3,19 +3,17 @@
 from typing import Any, Union
 
 from blake3 import blake3
 from typing import Protocol
 
 
 class Hasher(Protocol):
-    def hexdigest(self) -> str:
-        ...
+    def hexdigest(self) -> str: ...
 
-    def update(self, __data: Any) -> None:
-        ...
+    def update(self, __data: Any) -> None: ...
 
 
 def hasher(family: str = "sha256", **kwargs) -> Hasher:
     """
 
     :param family: str:  (Default value = "sha256")
     :param **kwargs:
```

## constellate/database/migration/migrationstep.py

```diff
@@ -160,17 +160,19 @@
 
                 pymodule, metadata = _read_file_metadata(file=mf)
                 validate_metadata(metadata=metadata)
 
                 default_parent = (
                     previous_mf.name
                     if previous_mf is not None
-                    else previous_migration_files[-1].name
-                    if len(previous_migration_files) > 0
-                    else None
+                    else (
+                        previous_migration_files[-1].name
+                        if len(previous_migration_files) > 0
+                        else None
+                    )
                 )
                 parent = next(iter(metadata.get("requires")), default_parent)
 
                 mark_behaviour = Mark.MARK_ACTIVITY
                 if not mf.name in DEFAULT_POST_APPLY_FILE_NAMES:
                     mark_behaviour |= Mark.MARK_MIGRATION
```

## constellate/database/sqlalchemy/sqlalchemypostgresql.py

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import functools
 from typing import Dict, Optional, Tuple
 
-from sqlalchemy import create_engine, inspect
+from sqlalchemy import create_engine, inspect, AsyncAdaptedQueuePool
 from sqlalchemy import event
 from sqlalchemy import text
 from sqlalchemy.engine.url import make_url
 from sqlalchemy.ext.asyncio import AsyncEngine
 from sqlalchemy.ext.asyncio import create_async_engine
 from sqlalchemy.pool import QueuePool
 from sqlalchemy.pool import NullPool
@@ -76,28 +76,27 @@
 
         scheme_driver = f"postgresql+{self._get_database_driver_name()}"
         connection_uri = f"{scheme_driver}://{credential_host}/{db_name}"
         connection_uri_plain = f"postgresql://{credential_host}/{db_name}"
         connection_uri_plain_schema = f"postgresql://{credential_host}/{db_name}?schema={db_schema}"
         connection_default_uri_plain = f"{scheme_driver}://{credential_host}/{db_name_default}"
 
-        pool_class = options.get("pool_class", QueuePool)
+        pool_class = options.get("pool_class", AsyncAdaptedQueuePool)
         pool_size = options.get("pool_connection_size", 10)
         pool_overflow_size = options.get("pool_connection_overflow_size", 5)
         pool_timeout = options.get("pool_connection_timeout", 30.0)
         pool_pre_ping = options.get("pool_pre_ping", False)
 
         kwargs = {
             "future": True,
             "echo": False,
             "echo_pool": False,
-            "poolclass": pool_class,
         }
 
-        if pool_class == QueuePool:
+        if pool_class == AsyncAdaptedQueuePool:
             kwargs.update(
                 {
                     "pool_size": pool_size,
                     "max_overflow": pool_overflow_size,
                     "pool_timeout": pool_timeout,
                     "pool_pre_ping": pool_pre_ping,
                 }
@@ -107,16 +106,20 @@
                 {
                     "pool_pre_ping": pool_pre_ping,
                 }
             )
         else:
             raise NotImplementedError("Unsupported pool class so far")
 
-        kwargs_async_engine = {}
-        kwargs_sync_engine = {}
+        kwargs_async_engine = {
+            "poolclass": AsyncAdaptedQueuePool if pool_class is QueuePool else pool_class,
+        }
+        kwargs_sync_engine = {
+            "poolclass": QueuePool if pool_class is AsyncAdaptedQueuePool else pool_class,
+        }
         if execution_options is not None:
             kwargs.update({"execution_options": execution_options})
         if application_name is not None:
             # asyncpg driver: 'server_settings' is a special argument to pass PG's client runtime parameters
             # src: https://magicstack.github.io/asyncpg/current/api/index.html#connection
             kwargs_async_engine.update(
                 connect_args={"server_settings": {"application_name": application_name}}
```

## constellate/database/sqlalchemy/expression/schema/create.py

```diff
@@ -34,15 +34,17 @@
         )
     )
 
     post_options = " ".join(
         filter(
             lambda x: x is not None,
             [
-                f"AUTHORIZATION {element._option_authorization}"
-                if element._option_authorization
-                else None
+                (
+                    f"AUTHORIZATION {element._option_authorization}"
+                    if element._option_authorization
+                    else None
+                )
             ],
         )
     )
 
     return f"CREATE SCHEMA {pre_options} {element.element} {post_options}"
```

## constellate/logger/log.py

```diff
@@ -10,14 +10,15 @@
 import pendulum
 from narration._handler.common.handler.base_handler import NarrationHandler
 from narration._misc.constants import DispatchMode
 from narration.constants import Backend
 from narration.narration import setup_server_handlers, setup_client_handlers
 
 from constellate.datatype.enum.enum import has_flag
+from constellate.logger.formatter.formatterfactory import builder
 from constellate.logger.handler.stringhandler import StringHandler
 from constellate.logger.loggers import Loggers
 from constellate.logger.logmode import LogMode
 
 
 class _LogDefault:
     LOGS_DIRECTORY = os.getcwd()
@@ -72,27 +73,39 @@
             fmt = fmt.replace(COLOR_MARKER, "") if remove_color else fmt
             colored = "colored" if not remove_color else "monocolor"
             key = f"console_{colored}_{name}"
             return (
                 key,
                 {
                     key: {
-                        "class": "logging.Formatter"
-                        if remove_color
-                        else "colorlog.ColoredFormatter",
+                        "()": ".".join([builder.__module__, builder.__name__]),
+                        "class_name": (
+                            "logging.Formatter" if remove_color else "colorlog.ColoredFormatter"
+                        ),
                         "format": fmt,
                         "date_fmt": "%Y-%m-%d %H:%M:%S",
+                        "defaults": {"exception_str": None},
                     }
                 },
             )
 
         def file_formatter(name=None, mode=None, normal_fmt=None, trace_fmt=None):
             key = f"fmt_{name}"
             fmt = trace_fmt if has_flag(mode, LogMode.DETAIL_TRACE) else normal_fmt
-            return (key, {key: {"class": "logging.Formatter", "format": fmt}})
+            return (
+                key,
+                {
+                    key: {
+                        "()": ".".join([builder.__module__, builder.__name__]),
+                        "class_name": "logging.Formatter",
+                        "format": fmt,
+                    },
+                    "defaults": {"exception_str": None},
+                },
+            )
 
         def rotating_file_handler(name=None, fmt_id=None, filename=None) -> Tuple[str, Dict]:
             key = f"rfhd_{name}"
             return (
                 key,
                 {
                     key: {
@@ -129,38 +142,39 @@
             mode=None,
             levelIfNotProd="DEBUG",
             propagate=False,
         ):
             return {
                 f"{name}": {
                     "handlers": handlers,
-                    "level": levelIFProd
-                    if has_flag(mode, LogMode.ENV_PRODUCTION)
-                    else levelIfNotProd,
+                    "level": (
+                        levelIFProd if has_flag(mode, LogMode.ENV_PRODUCTION) else levelIfNotProd
+                    ),
                     "propagate": propagate,
                 }
             }
 
+        exception_str_attribute = "%(exception_str)s" if sys.version_info >= (3, 10, 0) else ""
         console_fmt_id, console_fmt = console_formatter(
             name="console",
             mode=mode,
-            normal_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: {COLOR_MARKER}%(levelname)s: %(message)s",
-            trace_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(name)s: {COLOR_MARKER}%(levelname)s: %(message)s",
+            normal_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: {COLOR_MARKER}%(levelname)s: %(message)s {exception_str_attribute}",
+            trace_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(name)s: {COLOR_MARKER}%(levelname)s: %(message)s {exception_str_attribute}",
         )
         file_fmt_id, file_fmt = file_formatter(
             name="detailed",
             mode=mode,
-            normal_fmt="%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s",
-            trace_fmt="%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s",
+            normal_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s {exception_str_attribute}",
+            trace_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s {exception_str_attribute}",
         )
         root_file_fmt_id, root_file_fmt = file_formatter(
             name="root_detailed",
             mode=mode,
-            normal_fmt="%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s",
-            trace_fmt="%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(name)s: %(levelname)s: %(message)s",
+            normal_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s {exception_str_attribute}",
+            trace_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(name)s: %(levelname)s: %(message)s {exception_str_attribute}",
         )
 
         console_hd_id, console_hd = console_handler(name=f"{root_name}", formatter=console_fmt_id)
 
         config = {
             "disable_existing_loggers": False,
             "version": 1,
@@ -233,14 +247,30 @@
         mode: LogMode = _LogDefault.MODE,
         config_dict: Dict = None,
         template_config_dict: Dict = _LogDefault.TEMPLATE_CONFIG,
     ):
         Log._LOGS_DIRECTORY = log_dir_path
         Log._ROOT_LOGGER_NAME = root_logger_name
 
+        original_factory = logging.getLogRecordFactory()
+
+        def factory(
+            name, level, fn, lno, msg, args, exc_info, func=None, sinfo=None, **kwargs
+        ) -> logging.LogRecord:
+            record = original_factory(
+                name, level, fn, lno, msg, args, exc_info, func=func, sinfo=sinfo, **kwargs
+            )
+            if exc_info is not None and sys.version_info < (3, 11, 0):
+                record.exception_str = str(exc_info[1])
+            else:
+                record.exception_str = None
+            return record
+
+        logging.setLogRecordFactory(factory)
+
         # Load default logger config dict
         if config_dict is None:
             config_dict = Log.default_config_dict(
                 root_name=Log._ROOT_LOGGER_NAME, mode=mode, template=template_config_dict
             )
 
         # Load declarative config
```

## Comparing `constellate-0.8.1.dist-info/METADATA` & `constellate-0.8.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellate
-Version: 0.8.1
+Version: 0.8.3
 Summary: Constellate, a bunch of utilities aggregated over time.
 Home-page: https://github.com/davidandreoletti/constellate
 Author: David Andreoletti
 Author-email: none@provided.yet
 Keywords: constellate
 Classifier: License :: Other/Proprietary License
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `constellate-0.8.1.dist-info/RECORD` & `constellate-0.8.3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 constellate/compression/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/compression/zip/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/compression/zip/zip.py,sha256=AwVtgxvNOARp9gwbAafxix0lJ0a7hPCBr6kgGRbR24o,2575
 constellate/concurrency/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/concurrency/asyncio/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/concurrency/asyncio/tasks.py,sha256=ADhEd1q5zmPIok3h5NGkB08YDJAu9Sa5QBZBBPioKvU,3009
 constellate/concurrency/pebble/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-constellate/concurrency/pebble/pool_cleanup.py,sha256=1dn-rjqtWgYpMpd08Buywr1VKD0GGUU-r48RwRv6GOo,2695
+constellate/concurrency/pebble/pool_cleanup.py,sha256=XiILpWjsDjxdSW04OCA53U3_r9F3z6N94NU6jdJTYUA,2687
 constellate/concurrency/simple/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/concurrency/simple/simple.py,sha256=achTtC5Er6OIYzqsa0Qqt_0LN_NIb3t91bdhq69TFSQ,4056
 constellate/concurrency/std/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/concurrency/std/pool.py,sha256=lYn_lwxNaQoXeBfn3dmAVTpXV7-R13785WCnJCafKns,591
 constellate/constant/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/constant/concurrency.py,sha256=QpNcW6T9sW7HYiZB6tv5N-VlxMJpCZYpocykqanVo0A,250
 constellate/constant/debug.py,sha256=5Mpj67aYP_ZIty_jEv7fm-c0EUystIx-j-YelTDgT94,22
 constellate/constant/platform.py,sha256=hzfqb71-XD9EzELQ7AKjyd_strkzf4a2SQ9ChAmQLQ8,102
 constellate/container/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/container/orchestration/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/container/orchestration/k8s/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/container/orchestration/k8s/probe.py,sha256=0AlYV98QzETgwLzgGMUTKlft3Tp0k9vwLesGFwOdeh0,447
 constellate/cryptography/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/cryptography/digest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-constellate/cryptography/digest/hexadecimal.py,sha256=yisTed72VcPzcyRHURGMg_VM1mexaizXoOhF5oX2PUs,1809
+constellate/cryptography/digest/hexadecimal.py,sha256=NetP4mO177QYicmW_RK5JxubhBW2piEymb1FrOXV2Nk,1793
 constellate/database/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/common/databasetype.py,sha256=c-y6cFtZZv9ctiMeK5-SJc2yHfpua3KL14HIGgjhOjk,121
 constellate/database/migration/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/migration/constant.py,sha256=nJXkgDaTtC-8tjaoiijOyeehB-gd-HyRAZW4Yi2-qek,697
 constellate/database/migration/metadata.py,sha256=Ve5hW0FD9GnwEh-opRP_3fSb0MgUHnMfXoGgryqAl0M,2220
 constellate/database/migration/migrate.py,sha256=Sy-JnFv12UjKP7pOOXGHhVNFB8Do02PYq96o1bFKz1g,6720
 constellate/database/migration/migrationcontext.py,sha256=wlrb2yeiH1PYfey50xxfkWzuMsyJl7_r8vXwG8zKU4s,3429
-constellate/database/migration/migrationstep.py,sha256=3Ui5ibjFvculfhXc2PLGytYjfileWb5Avq0T1Uc6vrM,9565
+constellate/database/migration/migrationstep.py,sha256=n_WXLJqz29C9-0aRDyxaLYPkHKNeLkZAVrTdoMs9lXQ,9621
 constellate/database/migration/tablecontext.py,sha256=l_OgzN0aBfKG9SP3hD6smWkfIlFdJXW_ZdmQu8Cg_Sg,372
 constellate/database/migration/standard/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/migration/standard/base.py,sha256=hIgU9fxan-VNsJpyN0XwCruQWpaiR_U47d5bg67EKW8,445
 constellate/database/migration/standard/migrate.py,sha256=3M8-Al4kkB60pwptH-QRmSUATh3ANDrFzdq2PUvqreM,22344
 constellate/database/migration/standard/table.py,sha256=jKlpbCTw0zStDml1SLxSrYm6rnu_GIDSUjobj59uJV0,2492
 constellate/database/sparql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sparql/query.py,sha256=IB0j4jnrvkt0FlWRZDsPtb4-zzwBr1EBXnDaKOsDByY,606
@@ -47,30 +47,31 @@
 constellate/database/sqlalchemy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sqlalchemy/relationshiptype.py,sha256=tHtcOK7AQYX9DV2MDWyRi-QBXl_BnctEW_rBHUUteJE,180
 constellate/database/sqlalchemy/sqlalchemy.py,sha256=D1s8Rosg_GQZEsWOZimbqr9YI9P4oEZAfdwCt3uf7mI,32367
 constellate/database/sqlalchemy/sqlalchemydbconfig.py,sha256=4nXwVHYzFkH5fZKXqG6HEtTZLRMUT85m3by85vIoEpY,810
 constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py,sha256=fQ92AbA5tnJWohXuLJjahQ4y4w4Ll6ymouTB6fX5Qmk,1477
 constellate/database/sqlalchemy/sqlalchemyengineconfig.py,sha256=47myyLH3PSWDRViT_pxeQbZYr2pOYjGnLB_XWWOcCpY,1004
 constellate/database/sqlalchemy/sqlalchemymigrationconfig.py,sha256=S4r2-PuikjqYi9t4u18WQ6ptKEK4zWHKltCmSWysff0,215
-constellate/database/sqlalchemy/sqlalchemypostgresql.py,sha256=JdEz0xs-dhcpTMuAucJJBYl7o8rq_sVmIBdu7__TbyQ,12933
+constellate/database/sqlalchemy/sqlalchemypostgresql.py,sha256=rTvfrA0iNRm5axf9KpsAjjvrWfPchoxgTu-Jvli76xw,13143
 constellate/database/sqlalchemy/sqlalchemysqlite3.py,sha256=f3Meu1l7vA2AwoBU7GFvY4S1AKBNP6mJykEfJ828lRE,9931
 constellate/database/sqlalchemy/crud/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sqlalchemy/crud/cru.py,sha256=Bx37tvXkfOE3Ve35wfcMzJzr54LZ83GZu6YfZqmXEMs,6311
 constellate/database/sqlalchemy/exception/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sqlalchemy/exception/migrationexception.py,sha256=eXroMWkZ2rJDNewRIKtR7XZdNnoQWUGfjI3WDRZr-wg,46
 constellate/database/sqlalchemy/exception/vacumexception.py,sha256=RIltnU_e0WWhnk1KzFYe_T6o-Hj64oAS7MztFbKJGO4,42
 constellate/database/sqlalchemy/execution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sqlalchemy/execution/execute.py,sha256=pQf_ekzkR-ICDvuMcHpFaT8_8xIgOv9MbA6UdW_ttWg,7580
 constellate/database/sqlalchemy/expression/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sqlalchemy/expression/schema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-constellate/database/sqlalchemy/expression/schema/create.py,sha256=Mmp0HnH_r5kHBlchWuExxRPUZEJAkq1p6FCFsUj09i4,1462
+constellate/database/sqlalchemy/expression/schema/create.py,sha256=8rBUpGhhf38bHYcM6G3mpaHlVYkoXiBzXbR-SCPf2SA,1510
 constellate/database/sqlalchemy/expression/schema/drop.py,sha256=Zhkb38QQcX_d_UzmXQH39eCqixlq8ax6bHQzBlRPStM,1231
 constellate/database/sqlalchemy/expression/schema/setsearchpath.py,sha256=A34iE6rGNxQIpR8yVOUbo1A02HZGswJOpS1UyIUbQGU,1752
 constellate/database/sqlalchemy/expression/table/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sqlalchemy/expression/table/drop.py,sha256=2IQWMEE8-1gkYnK4LGDLcA9rgQ1ovDW_er1zbppVsjo,2344
+constellate/database/sqlalchemy/expression/table/lock.py,sha256=6Gp1sPS-ETTXDIU3b9z8H4aUb3ovwms3yqFpbAmHyVs,1641
 constellate/database/sqlalchemy/expression/table/presence.py,sha256=DD6rxlFHLhuMJ0WZwfibvhcJi0YE5GYFATukd4eq2mU,3576
 constellate/database/sqlalchemy/expression/table/truncate.py,sha256=jrSxy3StCgaPKyCz81ZWOScA6VHrHjqyVBHgT0lIfNc,1105
 constellate/database/sqlalchemy/session/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/database/sqlalchemy/session/multienginesession.py,sha256=xyRlw6FYTtgAa-6XK2aLArDa7v_HGNF6qqRFvMTCHMY,6196
 constellate/database/sqlalchemy/session/syncmultienginesession.py,sha256=aktRDMFK_cumf4WD6zgXwDMJmsawpJQnYXF1wJDo1Ic,3778
 constellate/database/sqlalchemy/session/syncmultiengineshardsession.py,sha256=4l-sNXK3f5Aq-EfhSaUScYwjEMOja3rjreHlI5-_9eI,3097
 constellate/database/sqlalchemy/session/binder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -104,18 +105,20 @@
 constellate/debug/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/debug/packages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/debug/packages/package.py,sha256=m8TrqkILjU_0lFSk1UuU3W6P-ltKKVWl1HmF3iZa1Dc,88
 constellate/debugger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/debugger/debugger.py,sha256=pWST3ICMmd4ZX5NYWCuY6-OzivuX1_bo00lVe_5gSpI,1374
 constellate/debugger/simple.py,sha256=_WJabiFCOn15wvPyNyf6rhr5y9YoGi7ce7w9FSUNU7o,737
 constellate/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-constellate/logger/log.py,sha256=9t2Lwx_4ATr1uTh7sjkBZsVccgRfMxQGWaj4SY0eUW4,18698
+constellate/logger/log.py,sha256=QdDii4Qaj0rCF59SCFQCDTWsDFS2CJt_IUm3M4Jr164,20086
 constellate/logger/loggers.py,sha256=w5Q_vnCi-VGnaEhx0bWAh0w2UwGu5wTcHN_MtQPwvwY,3980
 constellate/logger/logmode.py,sha256=YNLhf4DBr8cltl-Kc0mQv3o-O77-yM5ZWzaplTZhwW4,652
 constellate/logger/simple.py,sha256=qnfavIJddTIJFCXv8m834n7a_OhF4Ew-nU8JWUGPYkI,3050
+constellate/logger/formatter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+constellate/logger/formatter/formatterfactory.py,sha256=Cp2vjgUWcFE835Evm4Nmlp5u-jYUs0dRkqLpq1rTlew,785
 constellate/logger/handler/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/logger/handler/forwarderhandler.py,sha256=WnWHfrU6m3cei9oK-iBP6iVtY6yr5OFZbAYfH1Dthk0,562
 constellate/logger/handler/stringhandler.py,sha256=12un6DeWj74K1z3CjlWJxVa4o7v1K4iF4_aTbdW61fk,569
 constellate/network/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/network/download/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/network/url/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/network/url/unshortener.py,sha256=Hy3fmNdnn1CDZ_PT7tFSL_kp6Skd1H6IsNqXtcPql4s,248
@@ -139,32 +142,38 @@
 constellate/storage/filesystem/tmpfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/storage/filesystem/tmpfs/memory_tempfile.py,sha256=VmcVU1whlmZafMYUft6_n9pU5yZO5pCrFBsY1fz8_6w,6635
 constellate/storage/filesystem/tmpfs/rambacked.py,sha256=LCYYKL_EQ70O4GWfWA35voZGnhXoveZZjquuBH3x0wc,2631
 constellate/testing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/testing/mock/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/testing/mock/argv.py,sha256=pHiWqhiv6_p2sdbF8sdu6Cnk62--VWyDe5Pn_L3Cq5E,374
 constellate/thirdparty/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+constellate/thirdparty/numba/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+constellate/thirdparty/numba/progress/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+constellate/thirdparty/numba/progress/progress.py,sha256=eKDwewwvbf491zxS7r6exflFunjr2wm5gylWcC7-1_U,1074
 constellate/thirdparty/pandas/__init__.py,sha256=p5UqcdjZbBUlYtmkx4jRVM9S6QfqSkmFTe_LgVhJF7U,596
 constellate/thirdparty/pandas/accessor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/thirdparty/pandas/accessor/attribute_accessor.py,sha256=P7lFPqjWc3K36PKwPSmEEBFjm5xz4IwanUGa6KCzVag,3173
 constellate/thirdparty/pandas/extra/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/thirdparty/pandas/extra/sanitize/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/thirdparty/pandas/extra/sanitize/sanitize.py,sha256=KyRxOiydknLHhja8wIxaJj13HT1BmL6AvyNKYycwHVQ,11089
 constellate/thirdparty/pandas/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/thirdparty/pandas/io/sql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/thirdparty/pandas/io/sql/sqlalchemy.py,sha256=XuHlmYn2vK1UPPyNEk97kR0ipkwB50Z_tslXL4tPQbQ,2570
 constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py,sha256=pMIUqOJAipm3FBQhbpT7N9CT9R_4um2OqTQ4obtsQXY,565
 constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py,sha256=hZ3vLyfsdXfpYnrnwBzraL2vxBdhAzPnPmyUTJ6eBZw,1127
+constellate/thirdparty/pandas/operation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+constellate/thirdparty/pandas/operation/introspection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+constellate/thirdparty/pandas/operation/introspection/introspection.py,sha256=Ko14WebqG7U8y-rXBvrIYCoMA8L-JVdOj58EiqDi8YE,336
 constellate/thirdparty/pandas/validation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/thirdparty/pandas/validation/pandera.py,sha256=rKVK9ZzzvTLCJK83-uTtHgWV3Krireky-hv7Y6oww-0,624
 constellate/thirdparty/pandas/validation/validation.py,sha256=TJO-5JRN_-YaQhBOtiJCNYzV-nX2ssm46SMWJZvXXuo,6050
 constellate/thirdparty/pandera/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/thirdparty/pandera/inspector.py,sha256=n-KR1U578-GPSXrvM1tNiJXh5Kx8cbTSE3sBIm_2-J0,1660
 constellate/virtualization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/virtualization/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 constellate/virtualization/common/common.py,sha256=K77vjG8F-N4Xa1al5Ye2eCpN3dME6Dw6O8S0feg-N0k,214
 constellate/virtualization/docker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-constellate-0.8.1.dist-info/LICENSE,sha256=wTGLemWYvsXNo-EmHyZg5ooGz-HetNZb38UvkCPhqVA,47
-constellate-0.8.1.dist-info/METADATA,sha256=M6-mKPBsxeVAExqSLvBl6hDEhaI0ndRz3mHws7I4fIg,3470
-constellate-0.8.1.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-constellate-0.8.1.dist-info/top_level.txt,sha256=tOnbLhuFhTQkr9GBTMlDd77gRIwlHFHvjBRtaU3zKjU,12
-constellate-0.8.1.dist-info/RECORD,,
+constellate-0.8.3.dist-info/LICENSE,sha256=wTGLemWYvsXNo-EmHyZg5ooGz-HetNZb38UvkCPhqVA,47
+constellate-0.8.3.dist-info/METADATA,sha256=LmjoOmkp3XS_n-K97KGkYRJ8e-DDKmekhXyRS9E5msA,3470
+constellate-0.8.3.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+constellate-0.8.3.dist-info/top_level.txt,sha256=tOnbLhuFhTQkr9GBTMlDd77gRIwlHFHvjBRtaU3zKjU,12
+constellate-0.8.3.dist-info/RECORD,,
```

