# Comparing `tmp/bowtie_json_schema-2024.5.3.tar.gz` & `tmp/bowtie_json_schema-2024.5.4.tar.gz`

## Comparing `bowtie_json_schema-2024.5.3.tar` & `bowtie_json_schema-2024.5.4.tar`

### file list

```diff
@@ -1,249 +1,253 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.prettierrc.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/action.yml
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/noxfile.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/test-requirements.in
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/test-requirements.txt
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/__main__.py
--rw-r--r--   0        0        0    49047 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/_cli.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/_containers.py
--rw-r--r--   0        0        0    22576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/_core.py
--rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/_report.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/exceptions.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/py.typed
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/cli/info.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/Makefile
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/cli.rst
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/requirements.in
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/index.html
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/package.json
--rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/ImplementationReportView/EmbedBadges.css
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/conftest.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_github.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_implementation.py
--rw-r--r--   0        0        0    65083 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_integration.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_report.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/hatch_build.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/pyproject.toml
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.3/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/action.yml
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/noxfile.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/test-requirements.in
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/test-requirements.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/__main__.py
+-rw-r--r--   0        0        0    48740 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_cli.py
+-rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_commands.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_containers.py
+-rw-r--r--   0        0        0    22876 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_core.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_registry.py
+-rw-r--r--   0        0        0    11625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_report.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/py.typed
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/Makefile
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/cli.rst
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/index.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/requirements.in
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/index.html
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/package.json
+-rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/EmbedBadges.css
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-json-schema/Dockerfile
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-json-schema/bowtie_json_schema.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-json-schema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/conftest.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_cli.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_github.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_implementation.py
+-rw-r--r--   0        0        0    64845 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_integration.py
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_report.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/hatch_build.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.5.3/.gitpod.yml` & `bowtie_json_schema-2024.5.4/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/.pre-commit-config.yaml` & `bowtie_json_schema-2024.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/CONTRIBUTING.rst` & `bowtie_json_schema-2024.5.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/action.yml` & `bowtie_json_schema-2024.5.4/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/noxfile.py` & `bowtie_json_schema-2024.5.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/requirements.txt` & `bowtie_json_schema-2024.5.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/test-requirements.txt` & `bowtie_json_schema-2024.5.4/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/_cli.py` & `bowtie_json_schema-2024.5.4/bowtie/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Dialect,
     Example,
     Implementation,
     NoSuchImplementation,
     StartupFailed,
     Test,
     TestCase,
-    bowtie_schemas_registry,
+    validator_registry,
 )
 from bowtie.exceptions import DialectError, ProtocolError, UnsupportedDialect
 
 if TYPE_CHECKING:
     from collections.abc import (
         AsyncIterator,
         Awaitable,
@@ -413,15 +413,15 @@
         ctx: click.Context,
         param: click.Parameter | None,
         value: bool,
     ) -> None:
         if not value or ctx.resilient_parsing:
             return
         uri = f"tag:bowtie.report,2024:cli:{ctx.command.name}"
-        schema = bowtie_schemas_registry().contents(uri)
+        schema = validator_registry().schema(uri)
         # FIXME: Syntax highlight? But rich appears to be doing some bizarre
         #        line wrapping, even if I disable a bunch of random options
         #        (crop, no_wrap, word_wrap in Syntax, ...) which fails the
         #        integration tests.
         click.echo(json.dumps(schema, indent=2))
         ctx.exit()
 
@@ -738,26 +738,21 @@
         final_content += "### Results:"
         final_content += row_data[1]
 
     return final_content
 
 
 def make_validator(*more_schemas: SchemaResource):
-    from jsonschema.validators import (
-        validator_for,  # type: ignore[reportUnknownVariableType]
-    )
-
-    registry = more_schemas @ bowtie_schemas_registry()
+    validators = more_schemas @ validator_registry()
 
     def validate(instance: Any, schema: Schema) -> None:
-        Validator = validator_for(schema)  # type: ignore[reportUnknownVariableType]
         # FIXME: There's work to do upstream in referencing, but we still are
         # probably able to make this a bit better here as well
-        validator = Validator(schema, registry=registry)  # type: ignore[reportUnknownVariableType]
-        errors = list(validator.iter_errors(instance))  # type: ignore[reportUnknownVariableType]
+        validator = validators.for_schema(schema)
+        errors = list(validator.errors_for(instance))
         if errors:
             raise ProtocolError(errors=errors)  # type: ignore[reportPrivateUsage]
 
     return validate
 
 
 def do_not_validate(*ignored: SchemaResource) -> Callable[..., None]:
```

### Comparing `bowtie_json_schema-2024.5.3/bowtie/_commands.py` & `bowtie_json_schema-2024.5.4/bowtie/_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import re
 
 try:
     from typing import dataclass_transform
 except ImportError:
     from typing_extensions import dataclass_transform
 
-from attrs import asdict, field, frozen
+from attrs import asdict, field, filters, frozen
 from url import URL
 
 from bowtie import HOMEPAGE, exceptions
 
 if TYPE_CHECKING:
     from collections.abc import Awaitable, Callable, Mapping, Sequence
     from typing import ClassVar, Self
@@ -171,14 +171,16 @@
 
     @property
     def skipped(self) -> bool: ...
 
     @property
     def errored(self) -> bool: ...
 
+    def serializable(self) -> Message: ...
+
 
 @frozen
 class TestResult:
     errored = False
     skipped = False
 
     valid: bool
@@ -194,14 +196,17 @@
     def from_dict(cls, data: Message) -> AnyTestResult:
         if data.pop("skipped", False):
             return SkippedTest(**data)
         elif data.pop("errored", False):
             return ErroredTest(**data)
         return cls(valid=data["valid"])
 
+    def serializable(self) -> Message:
+        return asdict(self)
+
 
 TestResult.VALID = TestResult(valid=True)
 TestResult.INVALID = TestResult(valid=False)
 
 
 @frozen
 class SkippedTest:
@@ -216,14 +221,22 @@
     @classmethod
     def in_skipped_case(cls):
         """
         A skipped test which mentions it is part of an entirely skipped case.
         """
         return cls(message="All tests in this test case were skipped.")
 
+    def serializable(self) -> Message:
+        return asdict(
+            self,
+            filter=lambda k, v: (
+                k.name not in {"message", "issue_url"} or v is not None
+            ),
+        )
+
 
 @frozen
 class ErroredTest:
     context: dict[str, Any] = field(factory=dict)
 
     errored: bool = field(init=False, default=True)
     skipped: bool = False
@@ -235,28 +248,33 @@
         """
         A errored test which mentions it is part of an entirely errored case.
         """
         return cls(
             context=dict(message="All tests in this test case errored."),
         )
 
+    def serializable(self) -> Message:
+        return asdict(self)
+
 
 class AnyCaseResult(Protocol):
     @property
     def results(self) -> Sequence[AnyTestResult] | None: ...
 
     def result_for(self, i: int) -> AnyTestResult: ...
 
     def log(self, log: BoundLogger) -> None: ...
 
     def unsuccessful(
         self,
         expected: Sequence[bool | None],
     ) -> Unsuccessful: ...
 
+    def serializable(self) -> Message: ...
+
 
 def _case_result(seq: Seq, **data: Any) -> tuple[Seq, AnyCaseResult]:
     # FIXME: Remove passing seq through which is mostly to support future
     #        validation that the seq we got back is the right one
     match data:
         case {"errored": True, **data}:
             return seq, CaseErrored(**data)
@@ -325,16 +343,16 @@
         return self.result.unsuccessful(expected=self.expected)
 
     def log_and_be_serialized(self, log: BoundLogger) -> Mapping[str, Any]:
         self.result.log(log)
         return self.serializable()
 
     def serializable(self):
-        serializable = asdict(self)
-        serializable.update(serializable.pop("result"))
+        serializable = asdict(self, filter=filters.exclude("result"))
+        serializable.update(self.result.serializable())
         return serializable
 
 
 @frozen
 class CaseResult:
     """
     A test case which at least was run by the implementation.
@@ -342,14 +360,17 @@
 
     results: list[AnyTestResult]
 
     @classmethod
     def from_results(cls, results: list[dict[str, Any]]):
         return cls(results=[TestResult.from_dict(t) for t in results])
 
+    def serializable(self) -> Message:
+        return dict(results=[result.serializable() for result in self.results])
+
     def result_for(self, i: int) -> AnyTestResult:
         return self.results[i]
 
     def unsuccessful(self, expected: Sequence[bool | None]) -> Unsuccessful:
         skipped = errored = failed = 0
         for test, expecting in zip(self.results, expected):
             if test.skipped:
@@ -379,14 +400,17 @@
     caught: bool = field(default=True)
     errored: bool = field(default=True, init=False)
 
     @classmethod
     def uncaught(cls, message: str = "uncaught error", **context: Any):
         return cls(caught=False, message=message, context=context)
 
+    def serializable(self):
+        return asdict(self)
+
     def result_for(self, i: int) -> ErroredTest:
         return ErroredTest.in_errored_case()
 
     def unsuccessful(self, expected: Sequence[bool | None]) -> Unsuccessful:
         return Unsuccessful(errored=len(expected))
 
     def log(self, log: BoundLogger):
@@ -401,14 +425,22 @@
 
     results = None
 
     message: str | None = None
     issue_url: str | None = None
     skipped: bool = field(init=False, default=True)
 
+    def serializable(self):
+        return asdict(
+            self,
+            filter=lambda k, v: (
+                k.name not in {"message", "issue_url"} or v is not None
+            ),
+        )
+
     def result_for(self, i: int) -> SkippedTest:
         return SkippedTest.in_skipped_case()
 
     def unsuccessful(self, expected: Sequence[bool | None]) -> Unsuccessful:
         return Unsuccessful(skipped=len(expected))
 
     def log(self, log: BoundLogger):
```

### Comparing `bowtie_json_schema-2024.5.3/bowtie/_containers.py` & `bowtie_json_schema-2024.5.4/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/_core.py` & `bowtie_json_schema-2024.5.4/bowtie/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     STOP,
     CaseErrored,
     Dialect as DialectCommand,
     SeqCase,
     SeqResult,
     StartedDialect,
 )
+from bowtie._registry import ValidatorRegistry
 from bowtie.exceptions import DialectError, ProtocolError, UnsupportedDialect
 
 if TYPE_CHECKING:
     from collections.abc import (
         AsyncIterator,
         Callable,
         Iterable,
@@ -134,26 +135,25 @@
     def serializable(self):
         return str(self.uri)
 
     def specification(self, **kwargs: Any) -> Specification[SchemaResource]:
         return specification_with(str(self.uri), **kwargs)
 
     def current_dialect_resource(self) -> SchemaResource:
-        referrer = bowtie_schemas_registry().contents(
+        referrer = validator_registry().schema(
             "tag:bowtie.report,2024:ihop:schemaInCurrentDialect",
         )
 
         # it's of course unimportant what dialect is used for this referencing
         # schema, what matters is that the target dialect is applied
         from referencing.jsonschema import DRAFT202012
 
         return DRAFT202012.create_resource(
             {
                 "$id": referrer["$ref"],  # type: ignore[reportIndexIssue]
-                "$ref": str(self.uri),
             },
         )
 
 
 @frozen
 class NoSuchImplementation(Exception):
     """
@@ -764,10 +764,18 @@
             }
             for test in serializable.pop("tests")
         ]
         return serializable
 
 
 @cache
-def bowtie_schemas_registry() -> SchemaRegistry:
+def validator_registry() -> ValidatorRegistry:
     resources = referencing_loaders.from_traversable(files("bowtie.schemas"))
-    return EMPTY_REGISTRY.with_resources(resources).crawl()
+    registry = EMPTY_REGISTRY.with_resources(resources).crawl()
+
+    from referencing.jsonschema import DRAFT202012  # XXX
+
+    ignore_current_dialect = registry.with_resource(
+        uri="tag:bowtie.report,2023:ihop:__dialect__",
+        resource=DRAFT202012.create_resource({}),
+    )
+    return ValidatorRegistry.jsonschema(registry=ignore_current_dialect)
```

### Comparing `bowtie_json_schema-2024.5.3/bowtie/_report.py` & `bowtie_json_schema-2024.5.4/bowtie/_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from bowtie._commands import (
     Seq,
     SeqCase,
     SeqResult,
     StartedDialect,
     Unsuccessful,
 )
-from bowtie._core import Dialect, TestCase
+from bowtie._core import Dialect, TestCase, validator_registry
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Iterable, Mapping, Sequence
     from typing import Any, Literal, Self, TextIO
 
     from bowtie._commands import AnyTestResult, ImplementationId
     from bowtie._core import Example, ImplementationInfo, Test
@@ -215,30 +215,39 @@
             ordered = [v for _, v in sorted(results.items())]
             if ordered != [v for _, v in sorted(other_results[name].items())]:
                 return False
         return this == that
 
     @classmethod
     def from_input(cls, input: Iterable[Mapping[str, Any]]) -> Self:
+        # TODO: Support some interface for enabling/disabling validation.
+        validator = validator_registry().for_uri(
+            "tag:bowtie.report,2024:report",
+        )
+
         iterator = iter(input)
         header = next(iterator, None)
         if header is None:
             raise EmptyReport()
+        validator.validate(header)
         metadata = RunMetadata.from_dict(**header)
 
+        validator = metadata.dialect.current_dialect_resource() @ validator
+
         results: HashTrieMap[
             ImplementationId,
             HashTrieMap[Seq, SeqResult],
         ] = HashTrieMap.fromkeys(  # type: ignore[reportUnknownMemberType]
             (each.id for each in metadata.implementations),
             HashTrieMap(),
         )
         cases: HashTrieMap[Seq, TestCase] = HashTrieMap()
 
         for data in iterator:
+            validator.validate(data)
             match data:
                 case {"seq": seq, "case": case}:
                     if seq in cases:
                         raise DuplicateCase(seq)
                     case = TestCase.from_dict(dialect=metadata.dialect, **case)
                     cases = cases.insert(seq, case)
                     continue
```

### Comparing `bowtie_json_schema-2024.5.3/bowtie/_suite.py` & `bowtie_json_schema-2024.5.4/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/exceptions.py` & `bowtie_json_schema-2024.5.4/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/hypothesis.py` & `bowtie_json_schema-2024.5.4/bowtie/hypothesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 from bowtie import _commands
 from bowtie._core import (
     Dialect,
     Example,
     ImplementationInfo,
     Test,
     TestCase,
-    bowtie_schemas_registry,
+    validator_registry,
 )
 from bowtie._report import Report, RunMetadata
 
 
-def pattern_from(id):
+def pattern_from(uri):
     """
     Return a strategy which matches the pattern in the given schema.
     """
-    return from_regex(bowtie_schemas_registry().contents(id)["pattern"])
+    return from_regex(validator_registry().schema(uri)["pattern"])
 
 
 # FIXME: probably via hypothesis-jsonschema
 object_schemas = dictionaries(
     keys=text(),
     values=recursive(
         none() | booleans() | floats() | text(printable),
```

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/cli/info.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/run.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.93125%*

 * *Differences: {"'$defs'": "{'response': {'$ref': '#openResponse', delete: ['type', 'required', 'properties', "*

 * *            "'oneOf', '$defs']}, 'openResponse': OrderedDict([('$anchor', 'openResponse'), "*

 * *            "('type', 'object'), ('required', ['seq']), ('properties', OrderedDict([('seq', "*

 * *            "OrderedDict([('description', 'The unchanged sequence identifier originally provided "*

 * *            "in the request.'), ('$ref', 'tag:bowtie.report,2024:report:seq')]))])), ('oneOf', "*

 * *            "[OrderedDict([('$re […]*

```diff
@@ -1,11 +1,11 @@
 {
     "$defs": {
-        "response": {
-            "$anchor": "response",
+        "openResponse": {
+            "$anchor": "openResponse",
             "$defs": {
                 "errored": {
                     "$anchor": "errored",
                     "description": "Signal that the implementation encountered an internal error (which it caught). Additional context can be passed along (e.g. a traceback or exception detail).",
                     "properties": {
                         "context": {
                             "additionalProperties": true,
@@ -105,15 +105,19 @@
                     "$ref": "tag:bowtie.report,2024:report:seq",
                     "description": "The unchanged sequence identifier originally provided in the request."
                 }
             },
             "required": [
                 "seq"
             ],
-            "type": "object",
+            "type": "object"
+        },
+        "response": {
+            "$anchor": "response",
+            "$ref": "#openResponse",
             "unevaluatedProperties": false
         }
     },
     "$id": "tag:bowtie.report,2023:ihop:command:run",
     "description": "Sent to implementations for each test case.",
     "properties": {
         "case": {
```

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.5.4/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/data/dialects.json` & `bowtie_json_schema-2024.5.4/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/Makefile` & `bowtie_json_schema-2024.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/cli.rst` & `bowtie_json_schema-2024.5.4/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/conf.py` & `bowtie_json_schema-2024.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/contributing.rst` & `bowtie_json_schema-2024.5.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/github-actions.rst` & `bowtie_json_schema-2024.5.4/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/implementers.rst` & `bowtie_json_schema-2024.5.4/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/index.rst` & `bowtie_json_schema-2024.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/motd.txt` & `bowtie_json_schema-2024.5.4/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/requirements.txt` & `bowtie_json_schema-2024.5.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/docs/_static/logo.svg` & `bowtie_json_schema-2024.5.4/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/package.json` & `bowtie_json_schema-2024.5.4/frontend/package.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.5.4/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/tsconfig.json` & `bowtie_json_schema-2024.5.4/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/public/favicon.svg` & `bowtie_json_schema-2024.5.4/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/index.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.5.4/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.5.4/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.5.4/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.5.4/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.5.4/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.5.4/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.5.4/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.5.4/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.5.4/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.5.4/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/build.gradle`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,30 @@
     id 'java'
 }
 
 sourceSets {
     main {
         java {
             srcDir '.'
-            include 'BowtieJsonSchema.java'
+            include 'BowtieJsonSchemaFriend.java'
         }
     }
 }
 
 repositories {
-    mavenCentral()
+    maven {
+        mavenCentral()
+        url 'https://jitpack.io'
+    }
 }
 
 def harnessImplementation = [
-        group: 'dev.harrel',
-        name: 'json-schema',
-        version: '1.5.2'
+        group: 'net.jimblackler.jsonschemafriend',
+        name: 'core',
+        version: '0.12.4'
 ]
 def jsonProvider = [
         group: 'com.fasterxml.jackson.core',
         name: 'jackson-databind',
         version: '2.17.0'
 ]
 
@@ -35,16 +38,16 @@
 jar {
     archiveBaseName = 'harness'
     duplicatesStrategy = DuplicatesStrategy.EXCLUDE
     from {
         configurations.runtimeClasspath.collect { it.isDirectory() ? it : zipTree(it) }
     }
     manifest {
-        attributes "Main-Class": "BowtieJsonSchema"
+        attributes "Main-Class": "BowtieJsonSchemaFriend"
         attributes "Implementation-Group": harnessImplementation.group
-        attributes "Implementation-Name": harnessImplementation.name
+        attributes "Implementation-Name": "jsonschemafriend"
         attributes "Implementation-Version": harnessImplementation.version
         attributes "Provider-Group": jsonProvider.group
         attributes "Provider-Name": jsonProvider.name
         attributes "Provider-Version": jsonProvider.version
     }
 }
```

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.5.4/implementations/java-json-schema/build.gradle`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,27 @@
     id 'java'
 }
 
 sourceSets {
     main {
         java {
             srcDir '.'
-            include 'BowtieJsonSchemaFriend.java'
+            include 'BowtieJsonSchema.java'
         }
     }
 }
 
 repositories {
-    maven {
-        mavenCentral()
-        url 'https://jitpack.io'
-    }
+    mavenCentral()
 }
 
 def harnessImplementation = [
-        group: 'net.jimblackler.jsonschemafriend',
-        name: 'core',
-        version: '0.12.4'
+        group: 'dev.harrel',
+        name: 'json-schema',
+        version: '1.6.0'
 ]
 def jsonProvider = [
         group: 'com.fasterxml.jackson.core',
         name: 'jackson-databind',
         version: '2.17.0'
 ]
 
@@ -38,16 +35,16 @@
 jar {
     archiveBaseName = 'harness'
     duplicatesStrategy = DuplicatesStrategy.EXCLUDE
     from {
         configurations.runtimeClasspath.collect { it.isDirectory() ? it : zipTree(it) }
     }
     manifest {
-        attributes "Main-Class": "BowtieJsonSchemaFriend"
+        attributes "Main-Class": "BowtieJsonSchema"
         attributes "Implementation-Group": harnessImplementation.group
-        attributes "Implementation-Name": "jsonschemafriend"
+        attributes "Implementation-Name": harnessImplementation.name
         attributes "Implementation-Version": harnessImplementation.version
         attributes "Provider-Group": jsonProvider.group
         attributes "Provider-Name": jsonProvider.name
         attributes "Provider-Version": jsonProvider.version
     }
 }
```

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.5.4/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.5.4/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.5.4/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     validate,
 } from "@hyperjump/json-schema/draft-2020-12";
 import "@hyperjump/json-schema/draft-2019-09";
 import "@hyperjump/json-schema/draft-07";
 import "@hyperjump/json-schema/draft-06";
 import "@hyperjump/json-schema/draft-04";
 import packageJson from "./node_modules/@hyperjump/json-schema/package.json"
-assert {
+with {
     type: "json"
 };
 
 const hyperjump_version = packageJson.version;
 
 const stdio = readline.createInterface({
     input: process.stdin,
```

### Comparing `bowtie_json_schema-2024.5.3/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.5.4/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,32 +1,32 @@
 import readline from "readline/promises";
 import os from "os";
 import process from "process";
 import {
     Validator
 } from "jsonschema";
 import packageJson from "./node_modules/jsonschema/package.json"
-assert {
+with {
     type: "json"
 };
 
 import draft3 from "json-metaschema/draft-03-schema.json"
-assert {
+with {
     type: "json"
 };
 import draft4 from "json-metaschema/draft-04-schema.json"
-assert {
+with {
     type: "json"
 };
 import draft6 from "json-metaschema/draft-06-schema.json"
-assert {
+with {
     type: "json"
 };
 import draft7 from "json-metaschema/draft-07-schema.json"
-assert {
+with {
     type: "json"
 };
 
 const jsonschema_version = packageJson.version;
 
 const stdio = readline.createInterface({
     input: process.stdin,
```

### Comparing `bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.5.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.5.4/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.5.4/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.5.4/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.5.4/implementations/rust-boon/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM rust:1.77-slim AS builder
+FROM rust:1.78-slim AS builder
 
 RUN rustup target add x86_64-unknown-linux-musl
 RUN apt update && apt install -y musl-tools musl-dev build-essential gcc-x86-64-linux-gnu
 RUN update-ca-certificates
 
 WORKDIR /usr/src/myapp
 COPY . .
```

### Comparing `bowtie_json_schema-2024.5.3/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.5.4/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Dockerfile`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM rust:1.77-slim AS builder
+FROM rust:1.78-slim AS builder
 
 RUN rustup target add x86_64-unknown-linux-musl
 RUN apt update && apt install -y musl-tools musl-dev build-essential gcc-x86-64-linux-gnu
 RUN update-ca-certificates
 
 WORKDIR /usr/src/myapp
 COPY . .
```

### Comparing `bowtie_json_schema-2024.5.3/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/test_github.py` & `bowtie_json_schema-2024.5.4/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/test_hypothesis.py` & `bowtie_json_schema-2024.5.4/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/test_integration.py` & `bowtie_json_schema-2024.5.4/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 import asyncio
 import json as _json
 import os
 import sys
 import tarfile
 
 from aiodocker.exceptions import DockerError
-from jsonschema.validators import validator_for
 from markdown_it import MarkdownIt
 from markdown_it.tree import SyntaxTreeNode
 import pexpect
 import pytest
 import pytest_asyncio
 
 from bowtie._commands import ErroredTest, TestResult
 from bowtie._core import (
     Dialect,
     Implementation,
     Test,
     TestCase,
-    bowtie_schemas_registry,
+    validator_registry,
 )
 from bowtie._report import EmptyReport, InvalidReport, Report
 
 Test.__test__ = TestCase.__test__ = TestResult.__test__ = (
     False  # frigging py.test
 )
 
@@ -39,23 +38,18 @@
 WIDE_TERMINAL_ENV = dict(os.environ, TERMINAL_WIDTH="512")
 
 
 def tag(name: str):
     return f"bowtie-integration-tests/{name}"
 
 
-async def validate_command_output(command, output):
+async def command_validator(command):
     stdout, stderr = await bowtie(command, "--schema")
-    assert stderr == ""
-
-    schema = _json.loads(stdout)
-    Validator = validator_for(schema)
-    Validator.check_schema(schema)
-
-    Validator(schema, registry=bowtie_schemas_registry()).validate(output)
+    assert stderr == "", stderr
+    return validator_registry().for_schema(_json.loads(stdout))
 
 
 async def bowtie(*argv, stdin: str = "", exit_code=0, json=False):
     """
     Run a Bowtie subprocess asynchronously to completion.
 
     An exit code of `-1` means "any non-zero exit code".
@@ -1048,15 +1042,15 @@
         "json",
         "-i",
         envsonschema,
         json=True,
         exit_code=-1,  # because indeed envsonschema gets answers wrong.
     )
 
-    await validate_command_output(command="smoke", output=jsonout)
+    (await command_validator("smoke")).validate(jsonout)
     assert jsonout == [
         {
             "case": {
                 "description": "allow-everything",
                 "schema": {
                     "$schema": "https://json-schema.org/draft/2020-12/schema",
                 },
@@ -1297,15 +1291,15 @@
         "--format",
         "json",
         "-i",
         envsonschema,
     )
     jsonout = _json.loads(stdout)
 
-    await validate_command_output(command="info", output=jsonout)
+    (await command_validator("info")).validate(jsonout)
     assert jsonout == {
         "name": "envsonschema",
         "language": "python",
         "homepage": "https://github.com/bowtie-json-schema/bowtie",
         "issues": "https://github.com/bowtie-json-schema/bowtie/issues",
         "source": "https://github.com/bowtie-json-schema/bowtie",
         "dialects": [
@@ -1330,15 +1324,15 @@
         "-i",
         envsonschema,
         "-i",
         links,
     )
     jsonout = _json.loads(stdout)
 
-    await validate_command_output(command="info", output=jsonout)
+    (await command_validator("info")).validate(jsonout)
     assert jsonout == {
         tag("envsonschema"): {
             "name": "envsonschema",
             "language": "python",
             "homepage": "https://github.com/bowtie-json-schema/bowtie",
             "issues": "https://github.com/bowtie-json-schema/bowtie/issues",
             "source": "https://github.com/bowtie-json-schema/bowtie",
@@ -1621,15 +1615,15 @@
         "json",
         "--show",
         "failures",
         stdin=validate_stdout,
         json=True,
     )
 
-    await validate_command_output(command="summary", output=jsonout)
+    (await command_validator("summary")).validate(jsonout)
     assert jsonout == [
         [
             tag("envsonschema"),
             dict(failed=2, skipped=0, errored=0),
         ],
     ]
     assert stderr == ""
@@ -1797,15 +1791,15 @@
         "json",
         "--show",
         "validation",
         stdin=run_stdout,
         json=True,
     )
 
-    await validate_command_output(command="summary", output=jsonout)
+    (await command_validator("summary")).validate(jsonout)
     assert jsonout == [
         [
             {"type": "integer"},
             [
                 [
                     12,
                     {
@@ -1990,15 +1984,15 @@
         "json",
         "--show",
         "validation",
         stdin=run_stdout,
         json=True,
     )
 
-    await validate_command_output(command="summary", output=jsonout)
+    (await command_validator("summary")).validate(jsonout)
     assert jsonout == [
         [
             {"type": "integer"},
             [
                 [12, {tag("always_valid"): "valid"}],
                 [12.5, {tag("always_valid"): "valid"}],
             ],
```

### Comparing `bowtie_json_schema-2024.5.3/tests/test_report.py` & `bowtie_json_schema-2024.5.4/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/test_schemas.py` & `bowtie_json_schema-2024.5.4/tests/test_schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 """
 Test Bowtie's schemas for proper functionality.
 """
 
-from jsonschema.validators import validator_for
 import pytest
 
-from bowtie._core import Dialect, bowtie_schemas_registry
-
-DRAFT2020 = Dialect.by_alias()["2020"]
-REGISTRY = DRAFT2020.current_dialect_resource() @ bowtie_schemas_registry()
+from bowtie._core import validator_registry
 
 TEST = {
     "description": "a test",
     "instance": 37,
 }
 ANOTHER_TEST = {
     "description": "another test",
     "instance": "foo",
 }
 
 
 def errors(uri, instance):
-    schema = REGISTRY.contents(uri)
-    validator = validator_for(schema)(schema, registry=REGISTRY)
-    return list(validator.iter_errors(instance))
+    return list(validator_registry().for_uri(uri).errors_for(instance))
 
 
 @pytest.mark.parametrize(
     "valid, instance",
     [
         (
             True,
@@ -153,13 +147,9 @@
 def test_group(valid, instance):
     got = errors("tag:bowtie.report,2023:models:group", instance)
     assert valid == (not got), got
 
 
 def test_root_schema():
     canonical_url = "tag:bowtie.report,2023:ihop"
-    retrieved = REGISTRY.get_or_retrieve(canonical_url)
-    assert retrieved.value.contents["$id"] == canonical_url
-
-
-def test_nonempty():
-    assert REGISTRY
+    schema = validator_registry().schema(canonical_url)
+    assert schema["$id"] == canonical_url
```

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/cli/info.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.93125%*

 * *Differences: {"'$defs'": "{'response': {'$ref': '#openResponse', delete: ['type', 'required', 'properties', "*

 * *            "'oneOf', '$defs']}, 'openResponse': OrderedDict([('$anchor', 'openResponse'), "*

 * *            "('type', 'object'), ('required', ['seq']), ('properties', OrderedDict([('seq', "*

 * *            "OrderedDict([('description', 'The unchanged sequence identifier originally provided "*

 * *            "in the request.'), ('$ref', 'tag:bowtie.report,2024:report:seq')]))])), ('oneOf', "*

 * *            "[OrderedDict([('$re […]*

```diff
@@ -1,11 +1,11 @@
 {
     "$defs": {
-        "response": {
-            "$anchor": "response",
+        "openResponse": {
+            "$anchor": "openResponse",
             "$defs": {
                 "errored": {
                     "$anchor": "errored",
                     "description": "Signal that the implementation encountered an internal error (which it caught). Additional context can be passed along (e.g. a traceback or exception detail).",
                     "properties": {
                         "context": {
                             "additionalProperties": true,
@@ -105,15 +105,19 @@
                     "$ref": "tag:bowtie.report,2024:report:seq",
                     "description": "The unchanged sequence identifier originally provided in the request."
                 }
             },
             "required": [
                 "seq"
             ],
-            "type": "object",
+            "type": "object"
+        },
+        "response": {
+            "$anchor": "response",
+            "$ref": "#openResponse",
             "unevaluatedProperties": false
         }
     },
     "$id": "tag:bowtie.report,2023:ihop:command:run",
     "description": "Sent to implementations for each test case.",
     "properties": {
         "case": {
```

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/.gitignore` & `bowtie_json_schema-2024.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/LICENSE` & `bowtie_json_schema-2024.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/README.rst` & `bowtie_json_schema-2024.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/hatch_build.py` & `bowtie_json_schema-2024.5.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/pyproject.toml` & `bowtie_json_schema-2024.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.3/PKG-INFO` & `bowtie_json_schema-2024.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```

