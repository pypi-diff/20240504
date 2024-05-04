# Comparing `tmp/linkml-1.7.8.tar.gz` & `tmp/linkml-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.7.8.tar", max compression
+gzip compressed data, was "linkml-1.7.9.tar", max compression
```

## Comparing `linkml-1.7.8.tar` & `linkml-1.7.9.tar`

### file list

```diff
@@ -1,148 +1,149 @@
--rw-r--r--   0        0        0      535 2024-04-05 19:33:24.282387 linkml-1.7.8/LICENSE
--rw-r--r--   0        0        0     1369 2024-04-05 19:33:24.282387 linkml-1.7.8/README.md
--rw-r--r--   0        0        0     3663 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/__init__.py
--rw-r--r--   0        0        0      310 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/_version.py
--rw-r--r--   0        0        0    51006 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     4438 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/README.md
--rw-r--r--   0        0        0     1517 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     1956 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     2956 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     3787 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2538 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0     1014 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1466 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     3226 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     2705 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      635 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    34347 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5013 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10153 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     7696 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     5811 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/golanggen.py
--rw-r--r--   0        0        0     3437 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2151 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1729 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5324 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8644 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7728 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    27455 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/legacy/__init__.py
--rw-r--r--   0        0        0     3471 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    32926 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6450 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     7774 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    54458 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/owlgen.py
--rw-r--r--   0        0        0    14895 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/plantumlgen.py
--rw-r--r--   0        0        0     4720 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9750 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2290 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/protogen.py
--rw-r--r--   0        0        0      629 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/pydanticgen/__init__.py
--rw-r--r--   0        0        0    19506 2024-04-05 19:33:24.306387 linkml-1.7.8/linkml/generators/pydanticgen/array.py
--rw-r--r--   0        0        0      721 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/black.py
--rw-r--r--   0        0        0     2681 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/build.py
--rw-r--r--   0        0        0    29863 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/pydanticgen.py
--rw-r--r--   0        0        0    19990 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/template.py
--rw-r--r--   0        0        0      443 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/attribute.py.jinja
--rw-r--r--   0        0        0      834 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/base_model.py.jinja
--rw-r--r--   0        0        0      565 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/class.py.jinja
--rw-r--r--   0        0        0      240 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/conditional_import.py.jinja
--rw-r--r--   0        0        0      338 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/enum.py.jinja
--rw-r--r--   0        0        0      385 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/footer.py.jinja
--rw-r--r--   0        0        0      945 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/imports.py.jinja
--rw-r--r--   0        0        0      438 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/module.py.jinja
--rw-r--r--   0        0        0      532 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pydanticgen/templates/validator.py.jinja
--rw-r--r--   0        0        0    52915 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2973 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0      108 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shacl/__init__.py
--rw-r--r--   0        0        0     2193 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shacl/ifabsent_processor.py
--rw-r--r--   0        0        0     1827 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shacl/shacl_data_type.py
--rw-r--r--   0        0        0     8771 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9874 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6138 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      249 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2542 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1622 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9320 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    12343 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     6879 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/string_template.md
--rw-r--r--   0        0        0     2887 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4627 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     8577 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1614 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    12196 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/__init__.py
--rw-r--r--   0        0        0     4494 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17202 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     2085 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     5113 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/linter.py
--rw-r--r--   0        0        0    11502 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/linter/rules.py
--rw-r--r--   0        0        0       92 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     8622 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    26522 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/logical_model_transformer.py
--rw-r--r--   0        0        0      678 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/model_transformer.py
--rw-r--r--   0        0        0    18857 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5275 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/__init__.py
--rw-r--r--   0        0        0      742 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/cli_utils.py
--rw-r--r--   0        0        0     6283 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/converter.py
--rw-r--r--   0        0        0     3742 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/datautils.py
--rw-r--r--   0        0        0      472 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6912 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    38394 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/generator.py
--rw-r--r--   0        0        0      447 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5843 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0    21184 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/logictools.py
--rw-r--r--   0        0        0     9044 2024-04-05 19:33:24.310387 linkml-1.7.8/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4417 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9937 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    16761 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    46093 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    18447 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    17071 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2232 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1438 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/utils/validation.py
--rw-r--r--   0        0        0     5002 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/__init__.py
--rw-r--r--   0        0        0     7261 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/cli.py
--rw-r--r--   0        0        0     1165 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/__init__.py
--rw-r--r--   0        0        0     2616 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/delimited_file_loader.py
--rw-r--r--   0        0        0      809 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/json_loader.py
--rw-r--r--   0        0        0      559 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/loader.py
--rw-r--r--   0        0        0      525 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/passthrough_loader.py
--rw-r--r--   0        0        0      914 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/loaders/yaml_loader.py
--rw-r--r--   0        0        0      702 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/__init__.py
--rw-r--r--   0        0        0     2528 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/jsonschema_validation_plugin.py
--rw-r--r--   0        0        0     1985 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/pydantic_validation_plugin.py
--rw-r--r--   0        0        0     2308 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/recommended_slots_plugin.py
--rw-r--r--   0        0        0     3888 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/shacl_validation_plugin.py
--rw-r--r--   0        0        0     1548 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/plugins/validation_plugin.py
--rw-r--r--   0        0        0      870 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/report.py
--rw-r--r--   0        0        0     2732 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/validation_context.py
--rw-r--r--   0        0        0     5649 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validator/validator.py
--rw-r--r--   0        0        0      202 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validators/__init__.py
--rw-r--r--   0        0        0     7951 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4612 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    14905 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11611 2024-04-05 19:33:24.314387 linkml-1.7.8/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     7421 2024-04-05 19:33:54.086785 linkml-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 linkml-1.7.8/setup.py
--rw-r--r--   0        0        0     3724 1970-01-01 00:00:00.000000 linkml-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0      535 2024-05-04 00:39:38.434231 linkml-1.7.9/LICENSE
+-rw-r--r--   0        0        0     1369 2024-05-04 00:39:38.434231 linkml-1.7.9/README.md
+-rw-r--r--   0        0        0     3663 2024-05-04 00:39:38.454231 linkml-1.7.9/linkml/__init__.py
+-rw-r--r--   0        0        0      310 2024-05-04 00:39:38.454231 linkml-1.7.9/linkml/_version.py
+-rw-r--r--   0        0        0    51006 2024-05-04 00:39:38.454231 linkml-1.7.9/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     4438 2024-05-04 00:39:38.454231 linkml-1.7.9/linkml/generators/README.md
+-rw-r--r--   0        0        0     1517 2024-05-04 00:39:38.454231 linkml-1.7.9/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:39:38.454231 linkml-1.7.9/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     1956 2024-05-04 00:39:38.454231 linkml-1.7.9/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     3243 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     3787 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     3469 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1014 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1466 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     3226 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     2705 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    36396 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5013 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10153 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     7696 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     5811 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/golanggen.py
+-rw-r--r--   0        0        0     3437 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2149 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1729 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5324 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8638 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7757 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    27747 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/legacy/__init__.py
+-rw-r--r--   0        0        0     3471 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    34449 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6450 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     7774 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    57554 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0    14936 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/plantumlgen.py
+-rw-r--r--   0        0        0     4240 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9750 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2512 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/protogen.py
+-rw-r--r--   0        0        0      629 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/__init__.py
+-rw-r--r--   0        0        0    19506 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/array.py
+-rw-r--r--   0        0        0      721 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/black.py
+-rw-r--r--   0        0        0     2681 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/build.py
+-rw-r--r--   0        0        0    30138 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/pydanticgen.py
+-rw-r--r--   0        0        0    19990 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/template.py
+-rw-r--r--   0        0        0      443 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/attribute.py.jinja
+-rw-r--r--   0        0        0      834 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/base_model.py.jinja
+-rw-r--r--   0        0        0      565 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/class.py.jinja
+-rw-r--r--   0        0        0      240 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/conditional_import.py.jinja
+-rw-r--r--   0        0        0      338 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/enum.py.jinja
+-rw-r--r--   0        0        0      385 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/footer.py.jinja
+-rw-r--r--   0        0        0      945 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/imports.py.jinja
+-rw-r--r--   0        0        0      438 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/module.py.jinja
+-rw-r--r--   0        0        0      532 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pydanticgen/templates/validator.py.jinja
+-rw-r--r--   0        0        0    52879 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2959 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0      108 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/shacl/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/shacl/ifabsent_processor.py
+-rw-r--r--   0        0        0     1827 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/shacl/shacl_data_type.py
+-rw-r--r--   0        0        0     8800 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9930 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6138 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      249 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2542 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1622 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9320 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    12343 2024-05-04 00:39:38.458231 linkml-1.7.9/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     6879 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     3069 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4626 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     8577 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1614 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    12197 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     4494 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17202 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     2085 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     5113 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11502 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/linter/rules.py
+-rw-r--r--   0        0        0       92 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     8622 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    26522 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/transformers/logical_model_transformer.py
+-rw-r--r--   0        0        0      678 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/transformers/model_transformer.py
+-rw-r--r--   0        0        0    18857 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5275 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0       92 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/cli_utils.py
+-rw-r--r--   0        0        0     6283 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/converter.py
+-rw-r--r--   0        0        0     3742 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      472 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     8088 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/deprecation.py
+-rw-r--r--   0        0        0     6912 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    39100 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/generator.py
+-rw-r--r--   0        0        0      447 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5843 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0    21184 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/logictools.py
+-rw-r--r--   0        0        0     9044 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4417 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9937 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    16761 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    46093 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    18447 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    17071 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2232 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1438 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/utils/validation.py
+-rw-r--r--   0        0        0     5002 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/__init__.py
+-rw-r--r--   0        0        0     7605 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/cli.py
+-rw-r--r--   0        0        0     1165 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/loaders/__init__.py
+-rw-r--r--   0        0        0     2616 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/loaders/delimited_file_loader.py
+-rw-r--r--   0        0        0      809 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/loaders/json_loader.py
+-rw-r--r--   0        0        0      559 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/loaders/loader.py
+-rw-r--r--   0        0        0      525 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/loaders/passthrough_loader.py
+-rw-r--r--   0        0        0      914 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/loaders/yaml_loader.py
+-rw-r--r--   0        0        0      702 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/plugins/__init__.py
+-rw-r--r--   0        0        0     2634 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/plugins/jsonschema_validation_plugin.py
+-rw-r--r--   0        0        0     1985 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/plugins/pydantic_validation_plugin.py
+-rw-r--r--   0        0        0     2308 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/plugins/recommended_slots_plugin.py
+-rw-r--r--   0        0        0     3888 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/plugins/shacl_validation_plugin.py
+-rw-r--r--   0        0        0     1548 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/plugins/validation_plugin.py
+-rw-r--r--   0        0        0      898 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/report.py
+-rw-r--r--   0        0        0     2732 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/validation_context.py
+-rw-r--r--   0        0        0     5649 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validator/validator.py
+-rw-r--r--   0        0        0      202 2024-05-04 00:39:38.462231 linkml-1.7.9/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     7951 2024-05-04 00:39:38.466231 linkml-1.7.9/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4612 2024-05-04 00:39:38.466231 linkml-1.7.9/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:39:38.466231 linkml-1.7.9/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:39:38.466231 linkml-1.7.9/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    14905 2024-05-04 00:39:38.466231 linkml-1.7.9/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2024-05-04 00:39:38.466231 linkml-1.7.9/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11705 2024-05-04 00:39:38.466231 linkml-1.7.9/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     7492 2024-05-04 00:40:11.570252 linkml-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 linkml-1.7.9/setup.py
+-rw-r--r--   0        0        0     3724 1970-01-01 00:00:00.000000 linkml-1.7.9/PKG-INFO
```

### Comparing `linkml-1.7.8/LICENSE` & `linkml-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/README.md` & `linkml-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/__init__.py` & `linkml-1.7.9/linkml/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/PythonGenNotes.md` & `linkml-1.7.9/linkml/generators/PythonGenNotes.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/README.md` & `linkml-1.7.9/linkml/generators/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/__init__.py` & `linkml-1.7.9/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/common/type_designators.py` & `linkml-1.7.9/linkml/generators/common/type_designators.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/csvgen.py` & `linkml-1.7.9/linkml/generators/csvgen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generate CSVs
 """
 
 import os
-import sys
 from csv import DictWriter
 from dataclasses import dataclass
+from io import StringIO
 from typing import List, Optional, Set
 
 import click
 from linkml_runtime.linkml_model.meta import ClassDefinition, ClassDefinitionName
 from linkml_runtime.utils.formatutils import be, underscore
 
 from linkml._version import __version__
@@ -38,22 +38,28 @@
 
     closure: Optional[Set[ClassDefinitionName]] = None
     """List of classes to include in output"""
 
     writer: Optional[DictWriter] = None
     """Python dictwriter"""
 
+    _str_io: Optional[StringIO] = None
+    """String that the writer outputs to"""
+
     def __post_init__(self):
         super().__post_init__()
+        self._str_io = None
+
         self.generate_header()  # TODO: don't do this in initialization
 
-    def generate_header(self):
-        print(f"# metamodel_version: {self.schema.metamodel_version}")
+    def generate_header(self) -> str:
+        out = f"# metamodel_version: {self.schema.metamodel_version}"
         if self.schema.version:
-            print(f"# version: {self.schema.version}")
+            out = "\n".join([out, f"# version: {self.schema.version}"])
+        return out
 
     def visit_schema(self, classes: List[ClassDefinitionName] = None, **_) -> None:
         # Note: classes comes from the "root" argument
         self.closure = set()
 
         if classes is None:
             classes = []
@@ -61,16 +67,17 @@
         # Validate the supplied list of classes
         for clsname in classes:
             if clsname not in self.schema.classes:
                 raise ValueError(f"Unrecognized class: {clsname}")
             else:
                 self.closure.update(self.ancestors(self.schema.classes[clsname]))
 
+        self._str_io = StringIO()
         dialect: str = "excel" if self.format == "csv" else "excel-tab"
-        self.writer = DictWriter(sys.stdout, ["id", "mappings", "description"], dialect=dialect)
+        self.writer = DictWriter(self._str_io, ["id", "mappings", "description"], dialect=dialect)
         self.writer.writeheader()
 
     def visit_class(self, cls: ClassDefinition) -> bool:
         # TODO: find out what to do with mappings
         if not self.closure or cls.name in self.closure:
             self.writer.writerow(
                 {
@@ -79,14 +86,17 @@
                     "mappings": "",
                     "description": be(cls.description),
                 }
             )
             return True
         return False
 
+    def end_schema(self, **kwargs) -> str:
+        return self._str_io.getvalue()
+
 
 @shared_arguments(CsvGenerator)
 @click.command()
 @click.version_option(__version__, "-V", "--version")
 @click.option("--root", "-r", multiple=True, help="Class(es) to transform")
 def cli(yamlfile, root=None, **args):
     """Generate CSV/TSV file from LinkML model"""
```

### Comparing `linkml-1.7.8/linkml/generators/docgen/class.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/class.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,74 @@
+{% macro slot_relationship(element, slot) %}
+    {% set range_element = gen.name(schemaview.get_element(slot.range)) %}
+    {% set relation_label = gen.name(slot) %}
+    {{ gen.name(element) }} --> "{{ gen.cardinality(slot) }}" {{ range_element }} : {{ relation_label }}
+    click {{ range_element }} href "../{{ range_element }}"
+{% endmacro %}
+
 {% if schemaview.class_parents(element.name) and schemaview.class_children(element.name) %}
 ```{{ gen.mermaid_directive() }}
  classDiagram
     class {{ gen.name(element) }}
+    click {{ gen.name(element) }} href "../{{gen.name(element)}}"
       {% for s in schemaview.class_parents(element.name)|sort(attribute='name') -%}
         {{ gen.name(schemaview.get_element(s)) }} <|-- {{ gen.name(element) }}
+        click {{ gen.name(schemaview.get_element(s)) }} href "../{{gen.name(schemaview.get_element(s))}}"
       {% endfor %}
 
       {% for s in schemaview.class_children(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} <|-- {{ gen.name(schemaview.get_element(s)) }}
+        click {{ gen.name(schemaview.get_element(s)) }} href "../{{gen.name(schemaview.get_element(s))}}"
       {% endfor %}
       
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} --> {{ s.range }} : {{ gen.name(s) }}
+          {{ slot_relationship(element, s) }}
         {% endif %}
       {% endfor %}
 ```
 {% elif schemaview.class_parents(element.name) %}
 ```{{ gen.mermaid_directive() }}
  classDiagram
     class {{ gen.name(element) }}
+    click {{ gen.name(element) }} href "../{{gen.name(element)}}"
       {% for s in schemaview.class_parents(element.name)|sort(attribute='name') -%}
         {{ gen.name(schemaview.get_element(s)) }} <|-- {{ gen.name(element) }}
+        click {{ gen.name(schemaview.get_element(s)) }} href "../{{gen.name(schemaview.get_element(s))}}"
       {% endfor %}
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} --> {{ s.range }} : {{ gen.name(s) }}
+          {{ slot_relationship(element, s) }}
         {% endif %}
       {% endfor %}
 ```
 {% elif schemaview.class_children(element.name)  %}
 ```{{ gen.mermaid_directive() }}
  classDiagram
     class {{ gen.name(element) }}
+    click {{ gen.name(element) }} href "../{{gen.name(element)}}"
       {% for s in schemaview.class_children(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} <|-- {{ gen.name(schemaview.get_element(s)) }}
+        click {{ gen.name(schemaview.get_element(s)) }} href "../{{gen.name(schemaview.get_element(s))}}"
       {% endfor %}
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} --> {{ s.range }} : {{ gen.name(s) }}
+          {{ slot_relationship(element, s) }}
         {% endif %}
       {% endfor %}
 ```
 {% else %}
 ```{{ gen.mermaid_directive() }}
  classDiagram
     class {{ gen.name(element) }}
+    click {{ gen.name(element) }} href "../{{gen.name(element)}}"
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} --> {{ s.range }} : {{ gen.name(s) }}
+          {{ slot_relationship(element, s) }}
         {% endif %}
       {% endfor %}
 ```
 {% endif %}
```

### Comparing `linkml-1.7.8/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/enum.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/docgen/index.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/index.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/slot.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/docgen/subset.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/subset.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/docgen/type.md.jinja2` & `linkml-1.7.9/linkml/generators/docgen/type.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/docgen.py` & `linkml-1.7.9/linkml/generators/docgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -563,31 +563,68 @@
             if e.maximum_value is not None:
                 r = f"<= {e.maximum_value}"
         return r
 
     @staticmethod
     def cardinality(slot: SlotDefinition) -> str:
         """
-        Render combination of required, multivalued, and recommended as a range, e.g. 0..*
-        :param slot:
-        :return:
+        Render combination of required, multivalued, recommended, and exact_cardinality as a range,
+        according to Mermaid conventions. Considers 'required' and 'multivalued' to set defaults
+        for 'minimum_cardinality' and 'maximum_cardinality'.
+
+        Reference: https://mermaid.js.org/syntax/classDiagram.html#cardinality-multiplicity-on-relations
+
+        The different cardinality options are:
+        - 1 Only 1
+        - 0..1 Zero or One
+        - 1..* One or more
+        - * Many
+        - n n (where n>1)
+        - 0..n zero to n (where n>1)
+        - 1..n one to n (where n>1)
+        :param slot: SlotDefinition
+        :return: cardinality string as used in Mermaid diagrams
         """
-        if slot.required or slot.identifier:
-            min = "1"
+        if slot.exact_cardinality is not None:
+            cardinality = str(slot.exact_cardinality)  # handles 'n' case
         else:
-            min = "0"
-        if slot.multivalued:
-            max = "*"
-        else:
-            max = "1"
+            if slot.required or slot.identifier:
+                min_card = "1"
+            else:
+                min_card = str(slot.minimum_cardinality) if slot.minimum_cardinality is not None else "0"
+
+            if slot.multivalued:
+                max_card = "*"
+            else:
+                max_card = str(slot.maximum_cardinality) if slot.maximum_cardinality is not None else "1"
+
+            if min_card == "0":
+                if max_card == "1":
+                    cardinality = "0..1"  # handles '0..1' case
+                elif max_card == "*":
+                    cardinality = "*"  # handles '*' case
+                else:
+                    cardinality = f"0..{max_card}"  # handles '0..n' case
+            elif min_card == "1":
+                if max_card == "1":
+                    cardinality = "1"  # handles '1' case
+                elif max_card == "*":
+                    cardinality = "1..*"  # handles '1..*' case
+                else:
+                    cardinality = f"1..{max_card}"  # handles '1..n' case
+            else:
+                if max_card == "*":
+                    cardinality = f"{min_card}..*"  # handles 'n..*' case
+                else:
+                    cardinality = f"{min_card}..{max_card}"  # handles 'n..m' case
+
         if slot.recommended:
-            info = " _recommended_"
-        else:
-            info = ""
-        return f"{min}..{max}{info}"
+            cardinality += " _recommended_"
+
+        return cardinality
 
     def mermaid_directive(self) -> str:
         """
         Writes a mermaid directive. See <https://mermaid-js.github.io/mermaid/#/>_
 
         This comes after the triple-backtick.
 
@@ -928,14 +965,22 @@
     default=True,
     help="Render class table on index page in a hierarchically indented view",
 )
 @click.option(
     "--example-directory",
     help="Folder in which example files are found. These are used to make inline examples",
 )
+@click.option(
+    "-d",
+    "--include",
+    help="""
+Include LinkML Schema outside of imports mechanism.  Helpful in including deprecated classes and slots in a separate
+YAML, and including it when necessary but not by default (e.g. in documentation or for backwards compatibility)
+""",
+)
 @click.version_option(__version__, "-V", "--version")
 @click.command()
 def cli(
     yamlfile,
     directory,
     index_name,
     dialect,
```

### Comparing `linkml-1.7.8/linkml/generators/dotgen.py` & `linkml-1.7.9/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/erdiagramgen.py` & `linkml-1.7.9/linkml/generators/erdiagramgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/excelgen.py` & `linkml-1.7.9/linkml/generators/excelgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/golanggen.py` & `linkml-1.7.9/linkml/generators/golanggen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/golrgen.py` & `linkml-1.7.9/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/graphqlgen.py` & `linkml-1.7.9/linkml/generators/graphqlgen.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,46 +15,44 @@
     generatorname = os.path.basename(__file__)
     generatorversion = "0.1.1"
     valid_formats = ["graphql"]
     visit_all_class_slots = True
     uses_schemaloader = True
     requires_metamodel = False
 
-    def __post_init__(self):
-        super().__post_init__()
-        # TODO: move this
-        self.generate_header()
+    def visit_schema(self, **kwargs) -> str:
+        return self.generate_header()
 
-    def generate_header(self):
-        print(f"# metamodel_version: {self.schema.metamodel_version}")
+    def generate_header(self) -> str:
+        out = f"# metamodel_version: {self.schema.metamodel_version}\n"
         if self.schema.version:
-            print(f"# version: {self.schema.version}")
+            out += f"# version: {self.schema.version}\n"
+        return out
 
-    def visit_class(self, cls: ClassDefinition) -> bool:
+    def visit_class(self, cls: ClassDefinition) -> str:
         etype = "interface" if (cls.abstract or cls.mixin) and not cls.mixins else "type"
         mixins = ", ".join([camelcase(mixin) for mixin in cls.mixins])
-        print(f"{etype} {camelcase(cls.name)}" + (f" implements {mixins}" if mixins else ""))
-        print("  {")
-        return True
-
-    def end_class(self, cls: ClassDefinition) -> None:
-        print("  }")
-        print()
+        out = f"{etype} {camelcase(cls.name)}" + (f" implements {mixins}" if mixins else "")
+        out = "\n".join([out, "  {"])
+        return out
 
-    def visit_class_slot(self, cls: ClassDefinition, aliased_slot_name: str, slot: SlotDefinition) -> None:
+    def end_class(self, cls: ClassDefinition) -> str:
+        return "\n  }\n\n"
+
+    def visit_class_slot(self, cls: ClassDefinition, aliased_slot_name: str, slot: SlotDefinition) -> str:
         slotrange = (
             camelcase(slot.range)
             if slot.range in self.schema.classes or slot.range in self.schema.types or slot.range in self.schema.enums
             else "String"
         )
         if slot.multivalued:
             slotrange = f"[{slotrange}]"
         if slot.required:
             slotrange = slotrange + "!"
-        print(f"    {lcamelcase(aliased_slot_name)}: {slotrange}")
+        return f"\n    {lcamelcase(aliased_slot_name)}: {slotrange}"
 
 
 @shared_arguments(GraphqlGenerator)
 @click.command()
 @click.version_option(__version__, "-V", "--version")
 def cli(yamlfile, **args):
     """Generate graphql representation of a LinkML model"""
```

### Comparing `linkml-1.7.8/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.7.9/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/javagen.py` & `linkml-1.7.9/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/jsonldcontextgen.py` & `linkml-1.7.9/linkml/generators/jsonldcontextgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         self,
         base: Optional[Union[str, Namespace]] = None,
         output: Optional[str] = None,
         prefixes: Optional[bool] = True,
         flatprefixes: Optional[bool] = False,
         model: Optional[bool] = True,
         **_,
-    ) -> None:
+    ) -> str:
         if model is None:
             model = self.model
         context = JsonObj()
         if self.emit_metadata:
             comments = JsonObj()
             comments.description = "Auto generated by LinkML jsonld context generator"
             comments.generation_date = self.schema.generation_date
@@ -122,16 +122,16 @@
                 context_content[k] = v
             for k, v in self.slot_class_maps.items():
                 context_content[k] = v
         context["@context"] = context_content
         if output:
             with open(output, "w", encoding="UTF-8") as outf:
                 outf.write(as_json(context))
-        else:
-            print(as_json(context))
+
+        return str(as_json(context)) + "\n"
 
     def visit_class(self, cls: ClassDefinition) -> bool:
         class_def = {}
         cn = camelcase(cls.name)
         self.add_mappings(cls)
 
         self._build_element_id(class_def, cls.class_uri)
```

### Comparing `linkml-1.7.8/linkml/generators/jsonldgen.py` & `linkml-1.7.9/linkml/generators/jsonldgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     def visit_type(self, typ: TypeDefinition) -> None:
         self._visit(typ)
         typ.uri = self.namespaces.uri_for(typ.uri)
 
     def visit_subset(self, ss: SubsetDefinition) -> None:
         self._visit(ss)
 
-    def end_schema(self, context: str = None, **_) -> None:
+    def end_schema(self, context: str = None, **_) -> str:
         self._add_type(self.schema)
         base_prefix = self.default_prefix()
 
         # TODO: fix this, see https://github.com/linkml/linkml/issues/871
         # JSON LD adjusts context reference using '@base'.  If context is supplied and not a URI, generate an
         # absolute URI for it
         if context is None and self.format == "jsonld":
@@ -182,16 +182,17 @@
                 context[ci] = "file://" + context[ci]
 
         if self.format == "jsonld":
             self.schema["@context"] = context[0] if len(context) == 1 and not base_prefix else context
             if base_prefix:
                 self.schema["@context"].append({"@base": base_prefix})
         # json_obj["@id"] = self.schema.id
-        print(as_json(self.schema, indent="  "))
+        out = str(as_json(self.schema, indent="  ")) + "\n"
         self.schema = self.original_schema
+        return out
 
 
 @shared_arguments(JSONLDGenerator)
 @click.command()
 @click.option(
     "--context",
     multiple=True,
```

### Comparing `linkml-1.7.8/linkml/generators/jsonschemagen.py` & `linkml-1.7.9/linkml/generators/jsonschemagen.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 
     not_closed: Optional[bool] = True
     """If not closed, then an open-ended set of attributes can be instantiated for any object"""
 
     indent: int = 4
 
     inline: bool = False
+
     top_class: Optional[Union[ClassDefinitionName, str]] = None  # JSON object is one instance of this
     """Class instantiated by the root node of the document tree"""
 
     include_range_class_descendants: bool = False
     """If set, use an open world assumption and allow the range of a slot to be any descendant of the declared range.
     Note that if the range of a slot has a type designator, descendants will always be included.
     """
@@ -658,14 +659,22 @@
     "--title-from",
     type=click.Choice(["name", "title"], case_sensitive=False),
     default="name",
     help="""
 Specify from which slot are JSON Schema 'title' annotations generated.
 """,
 )
+@click.option(
+    "-d",
+    "--include",
+    help="""
+Include LinkML Schema outside of imports mechanism.  Helpful in including deprecated classes and slots in a separate
+YAML, and including it when necessary but not by default (e.g. in documentation or for backwards compatibility)
+""",
+)
 @click.version_option(__version__, "-V", "--version")
 def cli(yamlfile, **kwargs):
     """Generate JSON Schema representation of a LinkML model"""
     print(JsonSchemaGenerator(yamlfile, **kwargs).serialize(**kwargs))
 
 
 if __name__ == "__main__":
```

### Comparing `linkml-1.7.8/linkml/generators/linkmlgen.py` & `linkml-1.7.9/linkml/generators/linkmlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/markdowngen.py` & `linkml-1.7.9/linkml/generators/markdowngen.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
-from contextlib import redirect_stdout
+import re
 from dataclasses import dataclass
-from io import StringIO
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 import click
 from jsonasobj2 import JsonObj, values
 from linkml_runtime.linkml_model.meta import (
     ClassDefinition,
     ClassDefinitionName,
@@ -59,15 +58,15 @@
         self,
         directory: str = None,
         classes: Set[ClassDefinitionName] = None,
         image_dir: bool = False,
         index_file: str = "index.md",
         noimages: bool = False,
         **_,
-    ) -> None:
+    ) -> str:
         self.gen_classes = classes if classes else []
         for cls in self.gen_classes:
             if cls not in self.schema.classes:
                 raise ValueError("Unknown class name: {cls}")
         if self.gen_classes:
             self.gen_classes_neighborhood = self.neighborhood(list(self.gen_classes))
 
@@ -81,299 +80,324 @@
             if not noimages:
                 os.makedirs(self.image_directory, exist_ok=True)
         self.noimages = noimages
         if not self.no_types_dir:
             os.makedirs(os.path.join(directory, "types"), exist_ok=True)
 
         with open(self.exist_warning(directory, index_file), "w", encoding="UTF-8") as ixfile:
-            with redirect_stdout(ixfile):
-                self.frontmatter(f"{self.schema.name}")
+            items = []
+            items.append(self.frontmatter(f"{self.schema.name}"))
+            items.append(
                 self.para(
                     f"**metamodel version:** {self.schema.metamodel_version}\n\n**version:** {self.schema.version}"
                 )
-                self.para(be(self.schema.description))
+            )
+            items.append(self.para(be(self.schema.description)))
 
-                self.header(3, "Classes")
-                for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
-                    if not cls.is_a and not cls.mixin and self.is_secondary_ref(cls.name):
-                        self.class_hier(cls)
-
-                self.header(3, "Mixins")
-                for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
-                    if cls.mixin and self.is_secondary_ref(cls.name):
-                        self.class_hier(cls)
-
-                self.header(3, "Slots")
-                for slot in sorted(self.schema.slots.values(), key=lambda s: s.name):
-                    if not slot.is_a and self.is_secondary_ref(slot.name):
-                        self.pred_hier(slot)
-
-                self.header(3, "Enums")
-                for enu in sorted(self.schema.enums.values(), key=lambda e: e.name):
-                    self.enum_hier(enu)
-
-                self.header(3, "Subsets")
-                for subset in sorted(self.schema.subsets.values(), key=lambda s: s.name):
-                    self.bullet(self.subset_link(subset, use_desc=True), 0)
-
-                self.header(3, "Types")
-                self.header(4, "Built in")
-                for builtin_name in sorted(self.synopsis.typebases.keys()):
-                    self.bullet(f"**{builtin_name}**")
-                self.header(4, "Defined")
-                for typ in sorted(self.schema.types.values(), key=lambda t: t.name):
-                    if self.is_secondary_ref(typ.name):
-                        if typ.typeof:
-                            typ_typ = self.type_link(typ.typeof)
-                        else:
-                            typ_typ = f"**{typ.base}**"
+            items.append(self.header(3, "Classes"))
+            for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
+                if not cls.is_a and not cls.mixin and self.is_secondary_ref(cls.name):
+                    items.append(self.class_hier(cls))
+
+            items.append(self.header(3, "Mixins"))
+            for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
+                if cls.mixin and self.is_secondary_ref(cls.name):
+                    items.append(self.class_hier(cls))
+
+            items.append(self.header(3, "Slots"))
+            for slot in sorted(self.schema.slots.values(), key=lambda s: s.name):
+                if not slot.is_a and self.is_secondary_ref(slot.name):
+                    items.append(self.pred_hier(slot))
+
+            items.append(self.header(3, "Enums"))
+            for enu in sorted(self.schema.enums.values(), key=lambda e: e.name):
+                items.append(self.enum_hier(enu))
+
+            items.append(self.header(3, "Subsets"))
+            for subset in sorted(self.schema.subsets.values(), key=lambda s: s.name):
+                items.append(self.bullet(self.subset_link(subset, use_desc=True), 0))
+
+            items.append(self.header(3, "Types"))
+            items.append(self.header(4, "Built in"))
+            for builtin_name in sorted(self.synopsis.typebases.keys()):
+                items.append(self.bullet(f"**{builtin_name}**"))
+            items.append(self.header(4, "Defined"))
+            for typ in sorted(self.schema.types.values(), key=lambda t: t.name):
+                if self.is_secondary_ref(typ.name):
+                    if typ.typeof:
+                        typ_typ = self.type_link(typ.typeof)
+                    else:
+                        typ_typ = f"**{typ.base}**"
 
-                        self.bullet(self.type_link(typ, after_link=f" ({typ_typ})", use_desc=True))
+                    items.append(self.bullet(self.type_link(typ, after_link=f" ({typ_typ})", use_desc=True)))
+            items = [i for i in items if i is not None]
+            out = "\n".join(items) + "\n"
+            out = pad_heading(out)
+            ixfile.write(out)
+        return out
 
-    def visit_class(self, cls: ClassDefinition) -> bool:
+    def visit_class(self, cls: ClassDefinition) -> str:
         # allow client to relabel metamodel
         mixin_local_name = self.get_metamodel_slot_name("Mixin")
         class_local_name = self.get_metamodel_slot_name("Class")
 
         if self.gen_classes and cls.name not in self.gen_classes:
-            return False
+            return ""
 
         with open(self.exist_warning(self.dir_path(cls)), "w", encoding="UTF-8") as clsfile:
-            with redirect_stdout(clsfile):
-                class_curi = self.namespaces.uri_or_curie_for(str(self.namespaces._base), camelcase(cls.name))
-                class_uri = self.namespaces.uri_for(class_curi)
-                self.element_header(cls, cls.name, class_curi, class_uri)
-                print()
-                if not self.noyuml:
-                    if self.image_directory:
-                        yg = YumlGenerator(self)
-                        yg.serialize(
-                            classes=[cls.name],
-                            directory=self.image_directory,
-                            load_image=not self.noimages,
-                        )
-                        img_url = os.path.join("images", os.path.basename(yg.output_file_name))
-                    else:
-                        yg = YumlGenerator(self)
-                        img_url = (
-                            yg.serialize(classes=[cls.name])
-                            .replace("?", "%3F")
-                            .replace(" ", "%20")
-                            .replace("|", "&#124;")
-                        )
-
-                    print(f"[![img]({img_url})]({img_url})")
-
-                self.mappings(cls)
+            items = []
+            class_curi = self.namespaces.uri_or_curie_for(str(self.namespaces._base), camelcase(cls.name))
+            class_uri = self.namespaces.uri_for(class_curi)
+            items.append(self.element_header(cls, cls.name, class_curi, class_uri))
+            items.append("")
+            if not self.noyuml:
+                if self.image_directory:
+                    yg = YumlGenerator(self)
+                    yg.serialize(
+                        classes=[cls.name],
+                        directory=self.image_directory,
+                        load_image=not self.noimages,
+                    )
+                    img_url = os.path.join("images", os.path.basename(yg.output_file_name))
+                else:
+                    yg = YumlGenerator(self)
+                    img_url = (
+                        yg.serialize(classes=[cls.name]).replace("?", "%3F").replace(" ", "%20").replace("|", "&#124;")
+                    )
+
+                items.append(f"[![img]({img_url})]({img_url})")
+
+            if cls.id_prefixes:
+                items.append(self.header(2, "Identifier prefixes"))
+                for p in cls.id_prefixes:
+                    items.append(self.bullet(f"{p}"))
+
+            if cls.is_a is not None:
+                items.append(self.header(2, "Parents"))
+                items.append(self.bullet(f" is_a: {self.class_link(cls.is_a, use_desc=True)}"))
+            if cls.mixins:
+                items.append(self.header(2, f"Uses {mixin_local_name}"))
+                for mixin in cls.mixins:
+                    items.append(self.bullet(f" mixin: {self.class_link(mixin, use_desc=True)}"))
 
-                if cls.id_prefixes:
-                    self.header(2, "Identifier prefixes")
-                    for p in cls.id_prefixes:
-                        self.bullet(f"{p}")
-
-                if cls.is_a is not None:
-                    self.header(2, "Parents")
-                    self.bullet(f" is_a: {self.class_link(cls.is_a, use_desc=True)}")
-                if cls.mixins:
-                    self.header(2, f"Uses {mixin_local_name}")
-                    for mixin in cls.mixins:
-                        self.bullet(f" mixin: {self.class_link(mixin, use_desc=True)}")
-
-                if cls.name in self.synopsis.isarefs:
-                    self.header(2, "Children")
-                    for child in sorted(self.synopsis.isarefs[cls.name].classrefs):
-                        self.bullet(f"{self.class_link(child, use_desc=True)}")
-
-                if cls.name in self.synopsis.mixinrefs:
-                    self.header(2, f"{mixin_local_name} for")
-                    for mixin in sorted(self.synopsis.mixinrefs[cls.name].classrefs):
-                        self.bullet(f'{self.class_link(mixin, use_desc=True, after_link="(mixin)")}')
-
-                if cls.name in self.synopsis.classrefs:
-                    self.header(2, f"Referenced by {class_local_name}")
-                    for sn in sorted(self.synopsis.classrefs[cls.name].slotrefs):
-                        slot = self.schema.slots[sn]
-                        if slot.range == cls.name:
+            if cls.name in self.synopsis.isarefs:
+                items.append(self.header(2, "Children"))
+                for child in sorted(self.synopsis.isarefs[cls.name].classrefs):
+                    items.append(self.bullet(f"{self.class_link(child, use_desc=True)}"))
+
+            if cls.name in self.synopsis.mixinrefs:
+                items.append(self.header(2, f"{mixin_local_name} for"))
+                for mixin in sorted(self.synopsis.mixinrefs[cls.name].classrefs):
+                    items.append(self.bullet(f'{self.class_link(mixin, use_desc=True, after_link="(mixin)")}'))
+
+            if cls.name in self.synopsis.classrefs:
+                items.append(self.header(2, f"Referenced by {class_local_name}"))
+                for sn in sorted(self.synopsis.classrefs[cls.name].slotrefs):
+                    slot = self.schema.slots[sn]
+                    if slot.range == cls.name:
+                        items.append(
                             self.bullet(
                                 f" **{self.class_link(slot.domain)}** "
                                 f"*{self.slot_link(slot, add_subset=False)}*{self.predicate_cardinality(slot)}  "
                                 f"**{self.class_type_link(slot.range)}**"
                             )
+                        )
 
-                self.header(2, "Attributes")
-
-                # List all of the slots that directly belong to the class
-                slot_list = [slot for slot in [self.schema.slots[sn] for sn in cls.slots]]
-                own_slots = [slot for slot in slot_list if cls.name in slot.domain_of]
-                if own_slots:
-                    self.header(3, "Own")
-                    for slot in own_slots:
-                        self.slot_field(cls, slot)
-                        slot_list.remove(slot)
-
-                # List all of the inherited slots
-                ancestors = set(self.ancestors(cls))
-                inherited_slots = [slot for slot in slot_list if set(slot.domain_of).intersection(ancestors)]
-                if inherited_slots:
-                    self.header(3, "Inherited from " + cls.is_a + ":")
-                    for inherited_slot in inherited_slots:
-                        self.slot_field(cls, inherited_slot)
-                        slot_list.remove(inherited_slot)
-
-                # List all of the slots acquired through mixing
-                mixed_in_classes = set()
-                for mixin in cls.mixins:
-                    mixed_in_classes.add(mixin)
-                    mixed_in_classes.update(set(self.ancestors(self.schema.classes[mixin])))
-                for slot in slot_list:
-                    mixers = set(slot.domain_of).intersection(mixed_in_classes)
-                    for mixer in mixers:
-                        self.header(3, "Mixed in from " + mixer + ":")
-                        self.slot_field(cls, slot)
-
-                self.element_properties(cls)
+            items.append(self.header(2, "Attributes"))
 
-        return False
+            # List all of the slots that directly belong to the class
+            slot_list = [slot for slot in [self.schema.slots[sn] for sn in cls.slots]]
+            own_slots = [slot for slot in slot_list if cls.name in slot.domain_of]
+            if own_slots:
+                items.append(self.header(3, "Own"))
+                for slot in own_slots:
+                    items.append(self.slot_field(cls, slot))
+                    slot_list.remove(slot)
+
+            # List all of the inherited slots
+            ancestors = set(self.ancestors(cls))
+            inherited_slots = [slot for slot in slot_list if set(slot.domain_of).intersection(ancestors)]
+            if inherited_slots:
+                items.append(self.header(3, "Inherited from " + cls.is_a + ":"))
+                for inherited_slot in inherited_slots:
+                    items.append(self.slot_field(cls, inherited_slot))
+                    slot_list.remove(inherited_slot)
+
+            # List all of the slots acquired through mixing
+            mixed_in_classes = set()
+            for mixin in cls.mixins:
+                mixed_in_classes.add(mixin)
+                mixed_in_classes.update(set(self.ancestors(self.schema.classes[mixin])))
+            for slot in slot_list:
+                mixers = set(slot.domain_of).intersection(mixed_in_classes)
+                for mixer in mixers:
+                    items.append(self.header(3, "Mixed in from " + mixer + ":"))
+                    items.append(self.slot_field(cls, slot))
+
+            items.append(self.element_properties(cls))
+            out = "\n".join(items)
+            out = pad_heading(out)
+            clsfile.write(out)
+        return out
 
-    def visit_type(self, typ: TypeDefinition) -> None:
+    def visit_type(self, typ: TypeDefinition) -> str:
         with open(self.exist_warning(self.dir_path(typ)), "w", encoding="UTF-8") as typefile:
-            with redirect_stdout(typefile):
-                type_uri = typ.definition_uri
-                type_curie = self.namespaces.curie_for(type_uri)
-                self.element_header(typ, typ.name, type_curie, type_uri)
-
-                print("|  |  |  |")
-                print("| --- | --- | --- |")
-                if typ.typeof:
-                    print(f"| Parent type | | {self.class_type_link(typ.typeof)} |")
-                print(f"| Root (builtin) type | | **{typ.base}** |")
-                if typ.repr:
-                    print(f"| Representation | | {typ.repr} |")
-                self.element_properties(typ)
+            type_uri = typ.definition_uri
+            type_curie = self.namespaces.curie_for(type_uri)
+            out = self.element_header(typ, typ.name, type_curie, type_uri)
+
+            out = "\n".join([out, "|  |  |  |"])
+            out = "\n".join([out, "| --- | --- | --- |"])
+            if typ.typeof:
+                out = "\n".join([out, f"| Parent type | | {self.class_type_link(typ.typeof)} |"])
+            out = "\n".join([out, f"| Root (builtin) type | | **{typ.base}** |"])
+            if typ.repr:
+                out = "\n".join([out, f"| Representation | | {typ.repr} |"])
+            out += self.element_properties(typ)
+            out += "\n"
+            out = pad_heading(out)
+            typefile.write(out)
+        return out
 
-    def visit_slot(self, aliased_slot_name: str, slot: SlotDefinition) -> None:
+    def visit_slot(self, aliased_slot_name: str, slot: SlotDefinition) -> str:
         with open(self.exist_warning(self.dir_path(slot)), "w", encoding="UTF-8") as slotfile:
-            with redirect_stdout(slotfile):
-                slot_curie = self.namespaces.uri_or_curie_for(str(self.namespaces._base), underscore(slot.name))
-                slot_uri = self.namespaces.uri_for(slot_curie)
-                self.element_header(slot, aliased_slot_name, slot_curie, slot_uri)
-                self.mappings(slot)
-
-                self.header(2, "Domain and Range")
-                print(
+            items = []
+            slot_curie = self.namespaces.uri_or_curie_for(str(self.namespaces._base), underscore(slot.name))
+            slot_uri = self.namespaces.uri_for(slot_curie)
+            items.append(self.element_header(slot, aliased_slot_name, slot_curie, slot_uri))
+
+            items.append(self.header(2, "Domain and Range"))
+            items.append(
+                (
                     f"{self.class_link(slot.domain)} &#8594;{self.predicate_cardinality(slot)} "
                     f"{self.class_type_link(slot.range)}"
                 )
+            )
 
-                self.header(2, "Parents")
-                if slot.is_a:
-                    self.bullet(f" is_a: {self.slot_link(slot.is_a)}")
-
-                self.header(2, "Children")
-                if slot.name in sorted(self.synopsis.isarefs):
-                    for child in sorted(self.synopsis.isarefs[slot.name].slotrefs):
-                        self.bullet(f" {self.slot_link(child)}")
-
-                self.header(2, "Used by")
-                if slot.name in sorted(self.synopsis.slotrefs):
-                    for rc in sorted(self.synopsis.slotrefs[slot.name].classrefs):
-                        self.bullet(f"{self.class_link(rc)}")
-                if aliased_slot_name == "relation":
-                    if slot.subproperty_of:
-                        reifies = (
-                            self.slot_link(slot.subproperty_of)
-                            if slot.subproperty_of in self.schema.slots
-                            else slot.subproperty_of
-                        )
-                        self.bullet(f" reifies: {reifies}")
-                self.element_properties(slot)
+            items.append(self.header(2, "Parents"))
+            if slot.is_a:
+                items.append(self.bullet(f" is_a: {self.slot_link(slot.is_a)}"))
+
+            items.append(self.header(2, "Children"))
+            if slot.name in sorted(self.synopsis.isarefs):
+                for child in sorted(self.synopsis.isarefs[slot.name].slotrefs):
+                    items.append(self.bullet(f" {self.slot_link(child)}"))
+
+            items.append(self.header(2, "Used by"))
+            if slot.name in sorted(self.synopsis.slotrefs):
+                for rc in sorted(self.synopsis.slotrefs[slot.name].classrefs):
+                    items.append(self.bullet(f"{self.class_link(rc)}"))
+            if aliased_slot_name == "relation":
+                if slot.subproperty_of:
+                    reifies = (
+                        self.slot_link(slot.subproperty_of)
+                        if slot.subproperty_of in self.schema.slots
+                        else slot.subproperty_of
+                    )
+                    items.append(self.bullet(f" reifies: {reifies}"))
+            items.append(self.element_properties(slot))
+            out = "\n".join(items)
+            out = pad_heading(out)
+            slotfile.write(out)
+        return out
 
-    def visit_enum(self, enum: EnumDefinition) -> None:
+    def visit_enum(self, enum: EnumDefinition) -> str:
         with open(self.exist_warning(self.dir_path(enum)), "w", encoding="UTF-8") as enumfile:
-            with redirect_stdout(enumfile):
-                enum_curie = self.namespaces.uri_or_curie_for(str(self.namespaces._base), underscore(enum.name))
-                enum_uri = self.namespaces.uri_for(enum_curie)
-                self.element_header(obj=enum, name=enum.name, curie=enum_curie, uri=enum_uri)
-                self.element_properties(enum)
+            items = []
+            enum_curie = self.namespaces.uri_or_curie_for(str(self.namespaces._base), underscore(enum.name))
+            enum_uri = self.namespaces.uri_for(enum_curie)
+            items.append(self.element_header(obj=enum, name=enum.name, curie=enum_curie, uri=enum_uri))
+            items.append(self.element_properties(enum))
+            out = "\n".join(items)
+            out = pad_heading(out)
+            enumfile.write(out)
+        return out
 
-    def visit_subset(self, subset: SubsetDefinition) -> None:
+    def visit_subset(self, subset: SubsetDefinition) -> str:
         with open(self.exist_warning(self.dir_path(subset)), "w", encoding="UTF-8") as subsetfile:
-            with redirect_stdout(subsetfile):
-                curie = self.namespaces.uri_or_curie_for(str(self.namespaces._base), underscore(subset.name))
-                uri = self.namespaces.uri_for(curie)
-                self.element_header(obj=subset, name=subset.name, curie=curie, uri=uri)
-                # TODO: consider showing hierarchy within a subset
-                self.header(3, "Classes")
-                for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
-                    if not cls.mixin:
-                        if cls.in_subset and subset.name in cls.in_subset:
-                            self.bullet(self.class_link(cls, use_desc=True), 0)
-                self.header(3, "Mixins")
-                for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
-                    if cls.mixin:
-                        if cls.in_subset and subset.name in cls.in_subset:
-                            self.bullet(self.class_link(cls, use_desc=True), 0)
-                self.header(3, "Slots")
-                for slot in sorted(self.schema.slots.values(), key=lambda s: s.name):
-                    if slot.in_subset and subset.name in slot.in_subset:
-                        self.bullet(self.slot_link(slot, use_desc=True), 0)
-                self.header(3, "Types")
-                for type in sorted(self.schema.types.values(), key=lambda s: s.name):
-                    if type.in_subset and subset.name in type.in_subset:
-                        self.bullet(self.type_link(type, use_desc=True), 0)
-                self.header(3, "Enums")
-                for enum in sorted(self.schema.enums.values(), key=lambda s: s.name):
-                    if enum.in_subset and subset.name in enum.in_subset:
-                        self.bullet(self.enum_link(type, use_desc=True), 0)
-                self.element_properties(subset)
+            items = []
+            curie = self.namespaces.uri_or_curie_for(str(self.namespaces._base), underscore(subset.name))
+            uri = self.namespaces.uri_for(curie)
+            items.append(self.element_header(obj=subset, name=subset.name, curie=curie, uri=uri))
+            # TODO: consider showing hierarchy within a subset
+            items.append(self.header(3, "Classes"))
+            for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
+                if not cls.mixin:
+                    if cls.in_subset and subset.name in cls.in_subset:
+                        items.append(self.bullet(self.class_link(cls, use_desc=True), 0))
+            items.append(self.header(3, "Mixins"))
+            for cls in sorted(self.schema.classes.values(), key=lambda c: c.name):
+                if cls.mixin:
+                    if cls.in_subset and subset.name in cls.in_subset:
+                        items.append(self.bullet(self.class_link(cls, use_desc=True), 0))
+            items.append(self.header(3, "Slots"))
+            for slot in sorted(self.schema.slots.values(), key=lambda s: s.name):
+                if slot.in_subset and subset.name in slot.in_subset:
+                    items.append(self.bullet(self.slot_link(slot, use_desc=True), 0))
+            items.append(self.header(3, "Types"))
+            for type in sorted(self.schema.types.values(), key=lambda s: s.name):
+                if type.in_subset and subset.name in type.in_subset:
+                    items.append(self.bullet(self.type_link(type, use_desc=True), 0))
+            items.append(self.header(3, "Enums"))
+            for enum in sorted(self.schema.enums.values(), key=lambda s: s.name):
+                if enum.in_subset and subset.name in enum.in_subset:
+                    items.append(self.bullet(self.enum_link(enum, use_desc=True), 0))
+            items.append(self.element_properties(subset))
+            out = "\n".join(items)
+            out = pad_heading(out)
+            subsetfile.write(out)
+        return out
 
-    def element_header(self, obj: Element, name: str, curie: str, uri: str) -> None:
+    def element_header(self, obj: Element, name: str, curie: str, uri: str) -> str:
         if isinstance(obj, TypeDefinition):
             obj_type = "Type"
         elif isinstance(obj, ClassDefinition):
             obj_type = "Class"
         elif isinstance(obj, SlotDefinition):
             obj_type = "Slot"
         elif isinstance(obj, EnumDefinition):
             obj_type = "Enum"
         elif isinstance(obj, SubsetDefinition):
             obj_type = "Subset"
         else:
             obj_type = "Class"
 
         header_label = f"{obj_type}: ~~{name}~~ _(deprecated)_" if obj.deprecated else f"{obj_type}: {name}"
-        self.header(1, header_label)
+        out = self.header(1, header_label)
 
-        self.para(be(obj.description))
-        print(f"URI: [{curie}]({uri})")
-        print()
+        out += self.para(be(obj.description))
+        out = "\n".join([out, f"URI: [{curie}]({uri})", ""])
+        return out
 
-    def element_properties(self, obj: Element) -> None:
+    def element_properties(self, obj: Element) -> str:
         def identity(e: Any) -> Any:
             return e
 
         def prop_list(
             title: str,
             entries: Union[List, Dict],
             formatter: Optional[Callable[[Element], str]] = None,
-        ) -> None:
+        ) -> Optional[str]:
             if formatter is None:
                 formatter = identity
             if isinstance(entries, (dict, JsonObj)):
                 entries = list(values(entries))
             if entries:
-                print(f"| **{title}:** | | {formatter(entries[0])} |")
+                items = []
+                items.append(f"| **{title}:** | | {formatter(entries[0])} |")
                 for entry in entries[1:]:
-                    print(f"|  | | {formatter(entry)} |")
+                    items.append(f"|  | | {formatter(entry)} |")
+                return "\n".join(items)
 
-        def enum_list(title: str, obj: EnumDefinition) -> None:
+        def enum_list(title: str, obj: EnumDefinition) -> str:
             # This data is from the enum provided in the YAML
-            self.header(2, title)
-            print("| Text | Description | Meaning | Other Information |")
-            print("| :--- | :---: | :---: | ---: |")
+            items = []
+            items.append(self.header(2, title))
+            items.append("| Text | Description | Meaning | Other Information |")
+            items.append("| :--- | :---: | :---: | ---: |")
 
             for item, item_info in obj.permissible_values.items():
                 text = ""
                 desc = ""
                 meaning = ""
                 other = {}
                 for k in item_info:
@@ -384,74 +408,89 @@
                             desc = item_info[k]
                         elif k == "meaning":
                             meaning = item_info[k]
                         else:
                             other[k] = item_info[k]
                 if not other:
                     other = ""
-                print(f"| {text} | {desc} | {meaning} | {other} |")
+                items.append(f"| {text} | {desc} | {meaning} | {other} |")
+            return "\n".join(items)
+
+        items = []
 
-        attributes = StringIO()
-        with redirect_stdout(attributes):
-            prop_list("Aliases", obj.aliases)
+        items.append(prop_list("Aliases", obj.aliases))
+        items.append(
             prop_list(
                 "Local names",
                 obj.local_names,
                 lambda e: f"{e.local_name_value} ({e.local_name_source})",
             )
-            prop_list("Mappings", obj.mappings)
+        )
+        items.append(prop_list("Mappings", obj.mappings))
+        items.append(
             prop_list(
                 "Alt Descriptions",
                 obj.alt_descriptions,
                 lambda e: f"{e.description} ({e.source})",
             )
-            # todos
-            # notes
-            prop_list("Comments", obj.comments)
-            prop_list("Examples", obj.examples)
-            prop_list("In Subsets", obj.in_subset)
-            # from_schema
-            # imported_from
-            prop_list("See also", [f"[{v}]({v})" for v in obj.see_also])
-            prop_list("Exact Mappings", obj.exact_mappings)
-            prop_list("Close Mappings", obj.close_mappings)
-            prop_list("Narrow Mappings", obj.narrow_mappings)
-            prop_list("Broad Mappings", obj.broad_mappings)
-            prop_list("Related Mappings", obj.related_mappings)
-            #       - exact mappings
-            #       - close mappings
-            #       - related mappings
-            #       - deprecated element has exact replacement
-            #       - deprecated element has possible replacement
-            if type(obj) == EnumDefinition:
-                enum_list("Permissible Values", obj)
-
-        if attributes.getvalue():
-            self.header(2, "Other properties")
-            print("|  |  |  |")
-            print("| --- | --- | --- |")
-            print(attributes.getvalue())
-
-    def class_hier(self, cls: ClassDefinition, level=0) -> None:
-        self.bullet(self.class_link(cls, use_desc=True), level)
+        )
+        # todos
+        # notes
+        items.append(prop_list("Comments", obj.comments))
+        items.append(prop_list("Examples", obj.examples))
+        items.append(prop_list("In Subsets", obj.in_subset))
+        # from_schema
+        # imported_from
+        items.append(prop_list("See also", [f"[{v}]({v})" for v in obj.see_also]))
+        items.append(prop_list("Exact Mappings", obj.exact_mappings))
+        items.append(prop_list("Close Mappings", obj.close_mappings))
+        items.append(prop_list("Narrow Mappings", obj.narrow_mappings))
+        items.append(prop_list("Broad Mappings", obj.broad_mappings))
+        items.append(prop_list("Related Mappings", obj.related_mappings))
+
+        items = [i for i in items if i is not None]
+        if len(items) > 0:
+            header = "\n".join([self.header(2, "Other properties"), "|  |  |  |", "| --- | --- | --- |"])
+            items.insert(0, header)
+
+        #       - exact mappings
+        #       - close mappings
+        #       - related mappings
+        #       - deprecated element has exact replacement
+        #       - deprecated element has possible replacement
+        if type(obj) == EnumDefinition:
+            items.insert(0, enum_list("Permissible Values", obj))
+            items.insert(1, "\n")
+
+        out = "\n".join(items)
+        return out
+
+    def class_hier(self, cls: ClassDefinition, level=0) -> str:
+        items = []
+        items.append(self.bullet(self.class_link(cls, use_desc=True), level))
         if cls.name in sorted(self.synopsis.isarefs):
             for child in sorted(self.synopsis.isarefs[cls.name].classrefs):
-                self.class_hier(self.schema.classes[child], level + 1)
+                items.append(self.class_hier(self.schema.classes[child], level + 1))
+        return "\n".join(items) if items else None
 
-    def pred_hier(self, slot: SlotDefinition, level=0) -> None:
-        self.bullet(self.slot_link(slot, use_desc=True), level)
+    def pred_hier(self, slot: SlotDefinition, level=0) -> str:
+        items = []
+        items.append(self.bullet(self.slot_link(slot, use_desc=True), level))
         if slot.name in sorted(self.synopsis.isarefs):
             for child in sorted(self.synopsis.isarefs[slot.name].slotrefs):
-                self.pred_hier(self.schema.slots[child], level + 1)
+                items.append(self.pred_hier(self.schema.slots[child], level + 1))
+        return "\n".join(items) if items else None
 
-    def enum_hier(self, enum: EnumDefinition, level=0) -> None:
-        self.bullet(self.enum_link(enum, use_desc=True), level)
+    def enum_hier(self, enum: EnumDefinition, level=0) -> str:
+        items = []
+        items.append(self.bullet(self.enum_link(enum, use_desc=True), level))
         if enum.name in sorted(self.synopsis.isarefs):
             for child in sorted(self.synopsis.isarefs[enum.name].classrefs):
-                self.enum_hier(self.schema.enums[child], level + 1)
+                items.append(self.enum_hier(self.schema.enums[child], level + 1))
+        return "\n".join(items) if items else None
 
     def dir_path(
         self,
         obj: Union[ClassDefinition, SlotDefinition, TypeDefinition, EnumDefinition],
     ) -> str:
         filename = (
             self.formatted_element_name(obj)
@@ -461,23 +500,14 @@
                 if isinstance(obj, SlotDefinition)
                 else underscore(obj.name) if isinstance(obj, EnumDefinition) else camelcase(obj.name)
             )
         )
         subdir = "/types" if isinstance(obj, TypeDefinition) and not self.no_types_dir else ""
         return f"{self.directory}{subdir}/{filename}.md"
 
-    def mappings(self, obj: Union[SlotDefinition, ClassDefinition]) -> None:
-        # TODO: get rid of this?
-        # self.header(2, 'Mappings')
-        # for mapping in obj.mappings:
-        #     self.bullet(f"{self.xlink(mapping)} {self.to_uri(mapping)}")
-        # if obj.subclass_of:
-        #     self.bullet(self.xlink(obj.subclass_of))
-        pass
-
     def is_secondary_ref(self, en: str) -> bool:
         """Determine whether 'en' is the name of something in the neighborhood of the requested classes
 
         @param en: element name
         @return: True if 'en' is the name of a slot, class or type in the immediate neighborhood of of what we are
         building
         """
@@ -488,31 +518,35 @@
         elif en in self.schema.slots:
             return en in self.gen_classes_neighborhood.slotrefs
         elif en in self.schema.types:
             return en in self.gen_classes_neighborhood.typerefs
         else:
             return True
 
-    def slot_field(self, cls: ClassDefinition, slot: SlotDefinition) -> None:
-        self.bullet(f"{self.slot_link(slot)}{self.predicate_cardinality(slot)}")
+    def slot_field(self, cls: ClassDefinition, slot: SlotDefinition) -> str:
+        items = []
+        items.append(self.bullet(f"{self.slot_link(slot)}{self.predicate_cardinality(slot)}"))
         if slot.description:
-            self.bullet(f"Description: {slot.description}", level=1)
-        self.bullet(f"Range: {self.class_type_link(slot.range)}", level=1)
+            items.append(self.bullet(f"Description: {slot.description}", level=1))
+        items.append(self.bullet(f"Range: {self.class_type_link(slot.range)}", level=1))
         # if slot.subproperty_of:
         #     self.bullet(f'edge label: {self.slot_link(slot.subproperty_of)}', level=1)
         for example in slot.examples:
-            self.bullet(
-                f'Example: {getattr(example, "value", " ")} {getattr(example, "description", " ")}',
-                level=1,
+            items.append(
+                self.bullet(
+                    f'Example: {getattr(example, "value", " ")} {getattr(example, "description", " ")}',
+                    level=1,
+                )
             )
         # if slot.name not in self.own_slot_names(cls):
         #     self.bullet(f'inherited from: {self.class_link(slot.domain)}', level=1)
         if slot.in_subset:
             ssl = ",".join(slot.in_subset)
-            self.bullet(f"in subsets: ({ssl})", level=1)
+            items.append(self.bullet(f"in subsets: ({ssl})", level=1))
+        return "\n".join(items)
 
     def to_uri(self, uri_or_curie: str) -> str:
         """Return the URI for the slot if known"""
         if ":/" in uri_or_curie:
             return uri_or_curie
         elif self.namespaces.prefix_for(uri_or_curie) in self.namespaces:
             return self.namespaces.uri_for(uri_or_curie)
@@ -537,35 +571,36 @@
         if slot.multivalued:
             card_str = "1..\\*" if slot.required else "0..\\*"
         else:
             card_str = "1..1" if slot.required else "0..1"
         return f"  <sub><b>{card_str}</b></sub>"
 
     @staticmethod
-    def anchor(id_: str) -> None:
-        print(f'<a name="{id_}">', end="")
+    def anchor(id_: str) -> str:
+        return f'<a name="{id_}">'
 
     @staticmethod
-    def anchorend() -> None:
-        print("</a>")
+    def anchorend() -> str:
+        return "</a>"
 
-    def header(self, level: int, txt: str) -> None:
+    def header(self, level: int, txt: str) -> str:
         txt = self.get_metamodel_slot_name(txt)
-        print(f'\n{"#" * level} {txt}\n')
+        out = f'\n{"#" * level} {txt}\n'
+        return out
 
     @staticmethod
-    def para(txt: str) -> None:
-        print(f"\n{txt}\n")
+    def para(txt: str) -> str:
+        return f"\n{txt}\n"
 
     @staticmethod
-    def bullet(txt: str, level=0) -> None:
-        print(f'{"    " * level} * {txt}')
+    def bullet(txt: str, level=0) -> str:
+        return f'{"    " * level} * {txt}'
 
-    def frontmatter(self, thingtype: str, layout="default") -> None:
-        self.header(1, thingtype)
+    def frontmatter(self, thingtype: str, layout="default") -> str:
+        return self.header(1, thingtype)
         # print(f'---\nlayout: {layout}\n---\n')
 
     def bbin(self, obj: Element) -> str:
         """Boldify built in types
 
         @param obj: object name or id
         @return:
@@ -744,14 +779,19 @@
             else:
                 frag = id_.replace(":", "_")
                 base = "http://purl.obolibrary.org/obo/"
                 uri = base + frag
         return uri
 
 
+def pad_heading(text: str) -> str:
+    """Add an extra newline to a non-top-level header that doesn't have one preceding it"""
+    return re.sub(r"(?<!\n)\n##", "\n\n##", text)
+
+
 @shared_arguments(MarkdownGenerator)
 @click.command()
 @click.option("--dir", "-d", required=True, help="Output directory")
 @click.option("--classes", "-c", multiple=True, help="Class(es) to emit")
 @click.option("--map-fields", "-M", multiple=True, help="Map metamodel fields, e.g. slot=field")
 @click.option("--img", "-i", is_flag=True, help="Download YUML images to 'image' directory")
 @click.option("--index-file", "-I", help="Name of markdown file that holds index")
```

### Comparing `linkml-1.7.8/linkml/generators/namespacegen.py` & `linkml-1.7.9/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/oocodegen.py` & `linkml-1.7.9/linkml/generators/oocodegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/owlgen.py` & `linkml-1.7.9/linkml/generators/owlgen.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     SlotDefinition,
     SlotDefinitionName,
     TypeDefinition,
     TypeDefinitionName,
 )
 from linkml_runtime.utils.formatutils import camelcase, underscore
 from linkml_runtime.utils.introspection import package_schemaview
-from rdflib import OWL, RDF, XSD, BNode, Graph, Literal, URIRef
+from rdflib import DCTERMS, OWL, RDF, XSD, BNode, Graph, Literal, URIRef
 from rdflib.collection import Collection
 from rdflib.namespace import RDFS, SKOS
 from rdflib.plugin import Parser as rdflib_Parser
 from rdflib.plugin import plugins as rdflib_plugins
 
 from linkml import METAMODEL_NAMESPACE_NAME
 from linkml._version import __version__
@@ -143,14 +143,16 @@
 
     use_native_uris: bool = True
     """If True, use the definition_uris, otherwise use class_uris."""
 
     mixins_as_expressions: bool = None
     """EXPERIMENTAL: If True, use OWL existential restrictions to represent mixins"""
 
+    default_permissible_value_type: Union[str, URIRef] = field(default_factory=lambda: OWL.Class)
+
     slot_is_literal_map: Mapping[str, Set[bool]] = field(default_factory=lambda: defaultdict(set))
     """DEPRECATED: use node_owltypes"""
 
     node_owltypes: Mapping[Union[BNode, URIRef], Set[OWL_TYPE]] = field(default_factory=lambda: defaultdict(set))
     """rdfs:Datatype, owl:Thing"""
 
     simplify: bool = True
@@ -826,14 +828,36 @@
                 # )
             constraints_exprs, _ = self.add_constraints(typ, is_literal=True)
             eq_conjunctions.extend(constraints_exprs)
             ixn = self._intersection_of(eq_conjunctions)
             if ixn:
                 self.graph.add((type_uri, OWL.equivalentClass, ixn))
 
+    def _get_metatype(
+        self, element: Union[Definition, PermissibleValue], default_value: Optional[Union[str, URIRef]] = None
+    ) -> Optional[URIRef]:
+        impls = []
+        if isinstance(element, Definition):
+            impls.extend(element.implements)
+        if isinstance(element, PermissibleValue):
+            if "implements" in element.annotations:
+                ann = element.annotations["implements"]
+                v = ann.value
+                if not isinstance(v, list):
+                    v = [v]
+                impls.extend(v)
+        for impl in impls:
+            if impl.startswith("owl:"):
+                return OWL[impl.split(":")[1]]
+            if impl.startswith("rdfs:"):
+                return RDFS[impl.split(":")[1]]
+        if isinstance(default_value, str):
+            return URIRef(default_value)
+        return default_value
+
     def add_enum(self, e: EnumDefinition) -> None:
         g = self.graph
         enum_uri = self._enum_uri(e.name)
         g.add((enum_uri, RDF.type, OWL.Class))
         has_parent = False
         if e.is_a:
             self.graph.add((enum_uri, RDFS.subClassOf, self._enum_uri(e.is_a)))
@@ -852,50 +876,80 @@
                 (
                     enum_uri,
                     RDF.type,
                     URIRef(EnumDefinition.class_class_uri),
                 )
             )
         pv_uris = []
+        owl_types = []
+        enum_owl_type = self._get_metatype(e, self.default_permissible_value_type)
+
         for pv in e.permissible_values.values():
-            pv_uri = self._permissible_value_uri(pv, enum_uri, e)
-            pv_uris.append(pv_uri)
-            if pv_uri:
-                g.add((pv_uri, RDF.type, OWL.Class))
-                g.add((pv_uri, RDFS.label, Literal(pv.text)))
-                # TODO: make this configurable
-                g.add(
-                    (
-                        enum_uri,
-                        self.metamodel.namespaces[METAMODEL_NAMESPACE_NAME]["permissible_values"],
-                        pv_uri,
-                    )
+            pv_owl_type = self._get_metatype(pv, enum_owl_type)
+            owl_types.append(pv_owl_type)
+            if pv_owl_type == RDFS.Literal:
+                pv_node = Literal(pv.text)
+                if pv.meaning:
+                    logging.warning(f"Meaning on literal {pv.text} in {e.name} is ignored")
+            else:
+                pv_node = self._permissible_value_uri(pv, enum_uri, e)
+            pv_uris.append(pv_node)
+            g.add(
+                (
+                    enum_uri,
+                    self.metamodel.namespaces[METAMODEL_NAMESPACE_NAME]["permissible_values"],
+                    pv_node,
                 )
+            )
+            if not isinstance(pv_node, Literal):
+                g.add((pv_node, RDF.type, pv_owl_type))
+                g.add((pv_node, RDFS.label, Literal(pv.text)))
+                # TODO: make this configurable
                 # self._add_element_properties(pv_uri, pv)
                 if self.metaclasses:
-                    g.add((pv_uri, RDF.type, enum_uri))
+                    g.add((pv_node, RDF.type, enum_uri))
                 has_parent = False
                 if pv.is_a:
-                    self.graph.add((pv_uri, RDFS.subClassOf, self._permissible_value_uri(pv.is_a, enum_uri, e)))
+                    self.graph.add((pv_node, RDFS.subClassOf, self._permissible_value_uri(pv.is_a, enum_uri, e)))
                     has_parent = True
                 for mixin in sorted(pv.mixins):
                     parent = self._permissible_value_uri(mixin, enum_uri, e)
                     if self.mixins_as_expressions:
                         parent = self._some_values_from(self._metaslot_uri("mixins"), parent)
                     else:
                         has_parent = True
                     self.graph.add((enum_uri, RDFS.subClassOf, parent))
                 if not has_parent and self.add_root_classes:
-                    self.graph.add((pv_uri, RDFS.subClassOf, URIRef(PermissibleValue.class_class_uri)))
+                    self.graph.add((pv_node, RDFS.subClassOf, URIRef(PermissibleValue.class_class_uri)))
         if all([pv is not None for pv in pv_uris]):
-            self._union_of(pv_uris, node=enum_uri)
-            for pv_uri in pv_uris:
+            all_is_class = all([owl_type == OWL.Class for owl_type in owl_types])
+            all_is_individual = all([owl_type == OWL.NamedIndividual for owl_type in owl_types])
+            all_is_literal = all([owl_type == RDFS.Literal for owl_type in owl_types])
+            sub_pred = DCTERMS.isPartOf
+            combo_pred = None
+            if all_is_class or all_is_individual or all_is_literal:
+                if all_is_class:
+                    combo_pred = OWL.unionOf
+                    # self._union_of(pv_uris, node=enum_uri)
+                    sub_pred = RDFS.subClassOf
+                elif all_is_individual:
+                    combo_pred = OWL.oneOf
+                    # self._object_one_of(pv_uris, node=enum_uri)
+                    sub_pred = RDF.type
+                elif all_is_literal:
+                    combo_pred = OWL.oneOf
+                    # self._object_one_of(pv_uris, node=enum_uri)
+                    sub_pred = RDF.type
+                if combo_pred:
+                    self._boolean_expression(pv_uris, combo_pred, enum_uri, owl_types=set(owl_types))
+            for pv_node in pv_uris:
                 # this would normally be entailed, but we assert here so it is visible
                 # without reasoning
-                g.add((pv_uri, RDFS.subClassOf, enum_uri))
+                if not isinstance(pv_node, Literal):
+                    g.add((pv_node, sub_pred, enum_uri))
 
     def _add_rule(self, subject: Union[URIRef, BNode], rule: ClassRule, cls: ClassDefinition):
         if not self.use_swrl:
             return
         logging.warning("SWRL support is experimental and incomplete")
         head = []
         body = []
@@ -1026,14 +1080,17 @@
 
     def _intersection_of(self, exprs: List[Union[BNode, URIRef]], **kwargs) -> Optional[Union[BNode, URIRef]]:
         return self._boolean_expression(exprs, OWL.intersectionOf, **kwargs)
 
     def _union_of(self, exprs: List[Union[BNode, URIRef]], **kwargs) -> Optional[Union[BNode, URIRef]]:
         return self._boolean_expression(exprs, OWL.unionOf, **kwargs)
 
+    def _object_one_of(self, exprs: List[Union[BNode, URIRef]], **kwargs) -> Optional[Union[BNode, URIRef]]:
+        return self._boolean_expression(exprs, OWL.oneOf, **kwargs)
+
     def _exactly_one_of(self, exprs: List[Union[BNode, URIRef]]) -> Optional[Union[BNode, URIRef]]:
         if not exprs:
             raise ValueError("Must pass at least one")
         if len(exprs) == 1:
             return exprs[0]
         sub_exprs = []
         for i, x in enumerate(exprs):
@@ -1161,15 +1218,15 @@
         expanded = self.schemaview.get_uri(t, expand=True, native=native)
         if expanded.startswith("xsd:"):
             # TODO: fix upstream in schemaview; default_curi_maps is different on windows
             return XSD[expanded[4:]]
         return URIRef(expanded)
 
     def _permissible_value_uri(
-        self, pv: Union[str, EnumDefinition], enum_uri: str, enum_def: EnumDefinition = None
+        self, pv: Union[str, PermissibleValue], enum_uri: str, enum_def: EnumDefinition = None
     ) -> URIRef:
         if isinstance(pv, str):
             pv_name = pv
             if enum_def is None:
                 raise ValueError(f"Cannot find permissible value: {pv}, no enum definition provided")
             pvs = [pv for k, pv in enum_def.permissible_values.items() if k == pv_name]
             if len(pvs) != 1:
@@ -1178,14 +1235,18 @@
         if pv.meaning:
             return URIRef(self.schemaview.expand_curie(pv.meaning))
         else:
             return URIRef(enum_uri + "#" + pv.text.replace(" ", "+"))
 
     def slot_owl_type(self, slot: SlotDefinition) -> URIRef:
         sv = self.schemaview
+        if slot.implements:
+            for t in ["owl:AnnotationProperty", "owl:ObjectProperty", "owl:DatatypeProperty"]:
+                if t in slot.implements:
+                    return OWL[t.replace("owl:", "")]
         if slot.range is None:
             range = self.schemaview.schema.default_range
         else:
             range = slot.range
         if self.type_objects:
             return OWL.ObjectProperty
         is_literal_vals = self.slot_is_literal_map[slot.name]
@@ -1263,14 +1324,20 @@
 )
 @click.option(
     "--use-native-uris/--no-use-native-uris",
     default=True,
     show_default=True,
     help="Use model URIs rather than class/slot URIs",
 )
+@click.option(
+    "--default-permissible-value-type",
+    default=str(OWL.Class),
+    show_default=True,
+    help="Default OWL type for permissible values",
+)
 @click.version_option(__version__, "-V", "--version")
 def cli(yamlfile, metadata_profile: str, **kwargs):
     """Generate an OWL representation of a LinkML model
 
     Generate OWL using default parameters:
 
         gen-owl my_schema.yaml
```

### Comparing `linkml-1.7.8/linkml/generators/plantumlgen.py` & `linkml-1.7.9/linkml/generators/plantumlgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def visit_schema(
         self,
         classes: Set[ClassDefinitionName] = None,
         directory: Optional[str] = None,
         load_image: bool = True,
         **_,
-    ) -> None:
+    ) -> Optional[str]:
         if directory:
             os.makedirs(directory, exist_ok=True)
         if classes is not None:
             for cls in classes:
                 if cls not in self.schema.classes:
                     raise ValueError(f"Unknown class name: {cls}")
         self.class_generated = set()
@@ -106,18 +106,21 @@
                 if resp.ok:
                     with open(self.output_file_name, "wb") as f:
                         for chunk in resp.iter_content(chunk_size=2048):
                             f.write(chunk)
                 else:
                     self.logger.error(f"{resp.reason} accessing {plantuml_url}")
         else:
-            print(
-                "@startuml\nskinparam nodesep 10\n" + "\n".join(dedup_plantumlclassdef),
-                end="\n@enduml\n",
+            out = (
+                "@startuml\n"
+                "skinparam nodesep 10\n"
+                "hide circle\n"
+                "hide empty members\n" + "\n".join(dedup_plantumlclassdef) + "\n@enduml\n"
             )
+            return out
 
     def add_class(self, cn: ClassDefinitionName) -> str:
         """Define the class only if
         (a) it hasn't previously been generated and
         (b) it appears in the gen_classes list
 
         @param cn:
@@ -126,21 +129,19 @@
         slot_defs: List[str] = []
         if cn not in self.class_generated and (not self.focus_classes or cn in self.focus_classes):
             cls = self.schema.classes[cn]
             for slot in self.filtered_cls_slots(cn, all_slots=True, filtr=lambda s: s.range not in self.schema.classes):
                 if True or cn in slot.domain_of:
                     mod = self.prop_modifier(cls, slot)
                     slot_defs.append(
-                        '    {field} "'
+                        "    {field} "
                         + underscore(self.aliased_slot_name(slot))
-                        + '"'
                         + mod
-                        + ': "'
+                        + ": "
                         + underscore(slot.range)
-                        + '"'
                         + self.cardinality(slot)
                     )
             self.class_generated.add(cn)
         self.referenced.add(cn)
         cls = self.schema.classes[cn]
         if cls.abstract:
             class_type = "abstract"
```

### Comparing `linkml-1.7.8/linkml/generators/prefixmapgen.py` & `linkml-1.7.9/linkml/generators/prefixmapgen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Generate JSON-LD contexts
 
 """
 
-import csv
 import os
 from dataclasses import dataclass, field
 from typing import Dict, Optional, Set, Union
 
 import click
 from jsonasobj2 import JsonObj, as_json
 from linkml_runtime.linkml_model.meta import ClassDefinition, SlotDefinition
@@ -55,54 +54,47 @@
         if self.schema.default_prefix:
             dflt = self.namespaces.prefix_for(self.schema.default_prefix)
             if dflt:
                 self.default_ns = dflt
             if self.default_ns:
                 self.emit_prefixes.add(self.default_ns)
 
-    def end_schema(self, base: Optional[Union[str, Namespace]] = None, output: Optional[str] = None, **_) -> None:
+    def end_schema(self, base: Optional[Union[str, Namespace]] = None, output: Optional[str] = None, **_) -> str:
         context = JsonObj()
         if base:
             base = str(base)
             if "://" not in base:
                 self.context_body["@base"] = os.path.relpath(base, os.path.dirname(self.schema.source_file))
             else:
                 self.context_body["@base"] = base
         for prefix in sorted(self.emit_prefixes):
             context[prefix] = self.namespaces[prefix]
         for k, v in self.context_body.items():
             context[k] = v
         for k, v in self.slot_class_maps.items():
             context[k] = v
 
-        if output:
-            output_ext = output.split(".")[-1]
+        if self.format == "tsv":
+            mapping: Dict = {}  # prefix to IRI mapping
+            for prefix in sorted(self.emit_prefixes):
+                mapping[prefix] = self.namespaces[prefix]
+
+            items = []
+            for key, value in mapping.items():
+                items.append("\t".join([key, value]))
+            out = "\n".join(items)
 
-            if output_ext == "tsv":
-                mapping: Dict = {}
-                for prefix in sorted(self.emit_prefixes):
-                    mapping[prefix] = self.namespaces[prefix]
-
-                with open(output, "w", encoding="UTF-8") as outf:
-                    writer = csv.writer(outf, delimiter="\t")
-                    for key, value in mapping.items():
-                        writer.writerow([key, value])
-            else:
-                with open(output, "w", encoding="UTF-8") as outf:
-                    outf.write(as_json(context))
         else:
-            if self.format == "tsv":
-                mapping: Dict = {}  # prefix to IRI mapping
-                for prefix in sorted(self.emit_prefixes):
-                    mapping[prefix] = self.namespaces[prefix]
+            out = str(as_json(context))
 
-                for key, value in mapping.items():
-                    print(key, value, sep="\t")
-            else:
-                print(as_json(context))
+        if output:
+            with open(output, "w", encoding="UTF-8") as outf:
+                outf.write(out)
+
+        return out
 
     def visit_class(self, cls: ClassDefinition) -> bool:
         class_def = {}
         cn = camelcase(cls.name)
         self.add_mappings(cls)
         cls_prefix = self.namespaces.prefix_for(cls.class_uri)
         if not self.default_ns or not cls_prefix or cls_prefix != self.default_ns:
```

### Comparing `linkml-1.7.8/linkml/generators/projectgen.py` & `linkml-1.7.9/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/protogen.py` & `linkml-1.7.9/linkml/generators/protogen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from dataclasses import dataclass
+from typing import Optional
 
 import click
 from linkml_runtime.linkml_model.meta import ClassDefinition, SlotDefinition
 from linkml_runtime.utils.formatutils import camelcase, lcamelcase
 
 from linkml._version import __version__
 from linkml.utils.generator import Generator, shared_arguments
@@ -22,48 +23,52 @@
     valid_formats = ["proto"]
     visit_all_class_slots = True
     uses_schemaloader = True
 
     # ObjectVars
     relative_slot_num: int = 0
 
-    def __post_init__(self):
-        super().__post_init__()
-        self.generate_header()
-
-    def generate_header(self):
-        print(' syntax="proto3";')
-        print(" package")
-        print(f"// metamodel_version: {self.schema.metamodel_version}")
+    def visit_schema(self, **kwargs) -> Optional[str]:
+        return self.generate_header()
+
+    def generate_header(self) -> str:
+        items = []
+        items.append(' syntax="proto3";')
+        items.append(" package")
+        items.append(f"// metamodel_version: {self.schema.metamodel_version}")
         if self.schema.version:
-            print(f"// version: {self.schema.version}")
+            items.append(f"// version: {self.schema.version}")
+        out = "\n".join(items) + "\n"
+        return out
 
-    def visit_class(self, cls: ClassDefinition) -> bool:
+    def visit_class(self, cls: ClassDefinition) -> Optional[str]:
         if cls.mixin or cls.abstract or not cls.slots:
-            return False
+            return None
+        items = []
         if cls.description:
             for dline in cls.description.split("\n"):
-                print(f"// {dline}")
-        print(f"message {camelcase(cls.name)}")
-        print(" {")
+                items.append(f"// {dline}")
+        items.append(f"message {camelcase(cls.name)}")
+        items.append(" {")
+        out = "\n".join(items)
         self.relative_slot_num = 0
-        return True
+        return out
 
-    def end_class(self, cls: ClassDefinition) -> None:
-        print(" }")
+    def end_class(self, cls: ClassDefinition) -> str:
+        return "\n }\n"
 
-    def visit_class_slot(self, cls: ClassDefinition, aliased_slot_name: str, slot: SlotDefinition) -> None:
+    def visit_class_slot(self, cls: ClassDefinition, aliased_slot_name: str, slot: SlotDefinition) -> str:
         qual = "repeated " if slot.multivalued else ""
         slotname = lcamelcase(aliased_slot_name)
         slot_range = camelcase(slot.range)
         if slot.rank is None:
             # numbering of slots is important in the proto implementation
             # and should be determined by the rank param.
             slot.rank = 0
-        print(f" {qual} {lcamelcase(slot_range)} {(slotname)} = {slot.rank}")
+        return f"\n {qual} {lcamelcase(slot_range)} {(slotname)} = {slot.rank}"
 
 
 @shared_arguments(ProtoGenerator)
 @click.version_option(__version__, "-V", "--version")
 @click.command()
 def cli(yamlfile, **args):
     """Generate proto representation of LinkML model"""
```

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/__init__.py` & `linkml-1.7.9/linkml/generators/pydanticgen/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/array.py` & `linkml-1.7.9/linkml/generators/pydanticgen/array.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/black.py` & `linkml-1.7.9/linkml/generators/pydanticgen/black.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/build.py` & `linkml-1.7.9/linkml/generators/pydanticgen/build.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/pydanticgen.py` & `linkml-1.7.9/linkml/generators/pydanticgen/pydanticgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,21 @@
     ObjectImport,
     PydanticAttribute,
     PydanticBaseModel,
     PydanticClass,
     PydanticModule,
     TemplateModel,
 )
+from linkml.utils import deprecation_warning
 from linkml.utils.generator import shared_arguments
 from linkml.utils.ifabsent_functions import ifabsent_value_declaration
 
+if int(PYDANTIC_VERSION[0]) == 1:
+    deprecation_warning("pydantic-v1")
+
 
 def _get_pyrange(t: TypeDefinition, sv: SchemaView) -> str:
     pyrange = t.repr if t is not None else None
     if pyrange is None:
         pyrange = t.base
     if t.base == "XSDDateTime":
         pyrange = "datetime "
@@ -211,14 +215,19 @@
 
     # ObjectVars (identical to pythongen)
     gen_classvars: bool = True
     gen_slots: bool = True
     genmeta: bool = False
     emit_metadata: bool = True
 
+    def __post_init__(self):
+        super().__post_init__()
+        if int(self.pydantic_version) == 1:
+            deprecation_warning("pydanticgen-v1")
+
     def compile_module(self, **kwargs) -> ModuleType:
         """
         Compiles generated python code to a module
         :return:
         """
         pycode = self.serialize(**kwargs)
         try:
```

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/template.py` & `linkml-1.7.9/linkml/generators/pydanticgen/template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/templates/base_model.py.jinja` & `linkml-1.7.9/linkml/generators/pydanticgen/templates/base_model.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/templates/class.py.jinja` & `linkml-1.7.9/linkml/generators/pydanticgen/templates/class.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/templates/imports.py.jinja` & `linkml-1.7.9/linkml/generators/pydanticgen/templates/imports.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pydanticgen/templates/validator.py.jinja` & `linkml-1.7.9/linkml/generators/pydanticgen/templates/validator.py.jinja`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/pythongen.py` & `linkml-1.7.9/linkml/generators/pythongen.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,19 +181,16 @@
 
 # Enumerations
 {self.gen_enumerations()}
 
 # Slots
 {self.gen_slotdefs()}"""
 
-    def end_schema(self, **_):
-        print(
-            re.sub(r" +\n", "\n", self.gen_schema().replace("\t", "    ")).strip(" "),
-            end="",
-        )
+    def end_schema(self, **_) -> str:
+        return re.sub(r" +\n", "\n", self.gen_schema().replace("\t", "    ")).strip(" ")
 
     def gen_imports(self) -> str:
         list_ents = [f"from {k} import {', '.join(v)}" for k, v in self.gen_import_list().items()]
         return "\n".join(list_ents)
 
     def gen_import_list(self) -> Dict[str, List[str]]:
         """
```

### Comparing `linkml-1.7.8/linkml/generators/rdfgen.py` & `linkml-1.7.9/linkml/generators/rdfgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def __post_init__(self):
         self.original_schema = deepcopy(self.schema)
         super().__post_init__()
 
     def _data(self, g: Graph) -> str:
         return g.serialize(format="turtle" if self.format == "ttl" else self.format)
 
-    def end_schema(self, output: Optional[str] = None, context: str = None, **_) -> None:
+    def end_schema(self, output: Optional[str] = None, context: str = None, **_) -> str:
         gen = JSONLDGenerator(
             self.original_schema,
             format=JSONLDGenerator.valid_formats[0],
             metadata=self.emit_metadata,
             importmap=self.importmap,
         )
         # Iterate over permissible text strings making them URI compatible
@@ -63,19 +63,20 @@
         graph = Graph()
         graph.parse(
             data=jsonld_str,
             format="json-ld",
             base=str(self.namespaces._base),
             prefix=True,
         )
+        out = self._data(graph)
         if output:
             with open(output, "w", encoding="UTF-8") as outf:
-                outf.write(self._data(graph))
-        else:
-            print(self._data(graph))
+                outf.write(out)
+
+        return out
 
 
 @shared_arguments(RDFGenerator)
 @click.command()
 @click.option("-o", "--output", help="Output file name")
 @click.option(
     "--context",
```

### Comparing `linkml-1.7.8/linkml/generators/shacl/ifabsent_processor.py` & `linkml-1.7.9/linkml/generators/shacl/ifabsent_processor.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/shacl/shacl_data_type.py` & `linkml-1.7.9/linkml/generators/shacl/shacl_data_type.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/shaclgen.py` & `linkml-1.7.9/linkml/generators/shaclgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,19 @@
     uses_schemaloader = True
 
     def __post_init__(self) -> None:
         self.schemaview = SchemaView(self.schema)
         super().__post_init__()
         self.generate_header()
 
-    def generate_header(self):
-        print(f"# metamodel_version: {self.schema.metamodel_version}")
+    def generate_header(self) -> str:
+        out = f"\n# metamodel_version: {self.schema.metamodel_version}"
         if self.schema.version:
-            print(f"# version: {self.schema.version}")
+            out += f"\n# version: {self.schema.version}"
+        return out
 
     def serialize(self, **args) -> str:
         g = self.as_graph()
         data = g.serialize(format="turtle" if self.format in ["owl", "ttl"] else self.format)
         return data
 
     def as_graph(self) -> Graph:
```

### Comparing `linkml-1.7.8/linkml/generators/shexgen.py` & `linkml-1.7.9/linkml/generators/shexgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,20 +51,20 @@
 
         if METAMODEL_NAMESPACE_NAME not in self.namespaces:
             self.namespaces[METAMODEL_NAMESPACE_NAME] = METAMODEL_NAMESPACE
         self.meta = Namespace(
             self.namespaces.join(self.namespaces[METAMODEL_NAMESPACE_NAME], "")
         )  # URI for the metamodel
         self.base = Namespace(self.namespaces.join(self.namespaces._base, ""))  # Base URI for what is being modeled
-        self.generate_header()
 
-    def generate_header(self):
-        print(f"# metamodel_version: {self.schema.metamodel_version}")
+    def generate_header(self) -> str:
+        out = f"# metamodel_version: {self.schema.metamodel_version}\n"
         if self.schema.version:
-            print(f"# version: {self.schema.version}")
+            out += f"# version: {self.schema.version}\n"
+        return out
 
     def visit_schema(self, **_):
         # Adjust the schema context to include the base model URI
         context = self.shex["@context"]
         self.shex["@context"] = [context, {"@base": self.namespaces._base}]
         # Emit all of the type definitions
         for typ in self.schema.types.values():
@@ -76,14 +76,16 @@
                 elif typ_type_uri == SHEX.nonLiteral:
                     self.shapes.append(NodeConstraint(id=model_uri, nodeKind="nonliteral"))
                 else:
                     self.shapes.append(NodeConstraint(id=model_uri, datatype=self.namespaces.uri_for(typ.uri)))
             else:
                 typeof_uri = self._class_or_type_uri(typ.typeof)
                 self.shapes.append(Shape(id=model_uri, expression=typeof_uri))
+        if self.format != "json":
+            return self.generate_header()
 
     def visit_class(self, cls: ClassDefinition) -> bool:
         self.shape = Shape()
 
         # Start with all the parent classes, mixins and appytos
         struct_ref_list = [cls.is_a] if cls.is_a else []
         struct_ref_list += cls.mixins
@@ -156,31 +158,31 @@
                         # id=self._class_or_type_uri(slot.range),
                         values=values,
                     )
                     constraint.valueExpr = node_constraint
             else:
                 constraint.valueExpr = self._class_or_type_uri(slot.range)
 
-    def end_schema(self, output: Optional[str] = None, **_) -> None:
+    def end_schema(self, output: Optional[str] = None, **_) -> str:
         self.shex.shapes = self.shapes if self.shapes else [Shape()]
         shex = as_json_1(self.shex)
         if self.format == "rdf":
             g = Graph()
             g.parse(data=shex, format="json-ld", version="1.1")
             g.bind("owl", OWL)
             shex = g.serialize(format="turtle")
         elif self.format == "shex":
             g = Graph()
             self.namespaces.load_graph(g)
             shex = str(ShExC(self.shex, base=sfx(self.namespaces._base), namespaces=g))
+
         if output:
             with open(output, "w", encoding="UTF-8") as outf:
                 outf.write(shex)
-        else:
-            print(shex)
+        return shex
 
     def _class_or_type_uri(
         self,
         item: Union[TypeDefinition, ClassDefinition, ElementName],
         suffix: Optional[str] = "",
     ) -> URIorCURIE:
         # TODO: enums - figure this out
```

### Comparing `linkml-1.7.8/linkml/generators/sparqlgen.py` & `linkml-1.7.9/linkml/generators/sparqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.7.9/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.7.9/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/sqlalchemygen.py` & `linkml-1.7.9/linkml/generators/sqlalchemygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/sqltablegen.py` & `linkml-1.7.9/linkml/generators/sqltablegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/sssomgen.py` & `linkml-1.7.9/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/string_template.md` & `linkml-1.7.9/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/summarygen.py` & `linkml-1.7.9/linkml/generators/summarygen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Generate Summary Spreadsheets
 
 """
 
 import os
-import sys
 from csv import DictWriter
 from dataclasses import dataclass
+from io import StringIO
 from typing import Optional
 
 import click
 from linkml_runtime.linkml_model.meta import ClassDefinition, SlotDefinition
 from linkml_runtime.utils.formatutils import camelcase
 
 from linkml._version import __version__
@@ -24,17 +24,20 @@
     valid_formats = ["tsv"]
 
     dirname: str = None
     classtab: Optional[DictWriter] = None
     slottab: Optional[DictWriter] = None
     dialect: str = "excel-tab"
 
+    _str_io: Optional[StringIO] = None
+
     def visit_schema(self, **_) -> None:
+        self._str_io = StringIO()
         self.classtab = DictWriter(
-            sys.stdout,
+            self._str_io,
             [
                 "Class Name",
                 "Parent Class",
                 "YAML Class Name",
                 "Description",
                 "Flags",
                 "Slot Name",
@@ -75,14 +78,17 @@
                 "YAML Slot Name": slot.name if slot.name != aliased_slot_name else "",
                 "Range": ref + self.class_or_type_name(slot.range),
                 "Slot Description": slot.description,
                 "URI": slot.slot_uri,
             }
         )
 
+    def end_schema(self, **kwargs) -> Optional[str]:
+        return self._str_io.getvalue()
+
 
 @shared_arguments(SummaryGenerator)
 @click.version_option(__version__, "-V", "--version")
 @click.command()
 def cli(yamlfile, **args):
     """Generate TSV summary files for viewing in Excel and the like"""
     print(SummaryGenerator(yamlfile, **args).serialize(**args))
```

### Comparing `linkml-1.7.8/linkml/generators/terminusdbgen.py` & `linkml-1.7.9/linkml/generators/terminusdbgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
     raw_additions: List = None
     clswq: str = None
 
     def visit_schema(self, inline: bool = False, **kwargs) -> None:
         self.classes = []
         self.raw_additions = []
 
-    def end_schema(self, **_) -> None:
-        print(json.dumps(WQ().woql_and(*self.classes, *self.raw_additions).to_dict(), indent=2))
+    def end_schema(self, **_) -> str:
+        return json.dumps(WQ().woql_and(*self.classes, *self.raw_additions).to_dict(), indent=2)
 
     def visit_class(self, cls: ClassDefinition) -> bool:
         self.clswq = WQ().add_class(camelcase(cls.name)).label(camelcase(cls.name)).description(be(cls.description))
         if cls.is_a:
             self.clswq.parent(camelcase(cls.is_a))
         if cls.abstract:
             self.clswq.abstract()
```

### Comparing `linkml-1.7.8/linkml/generators/typescriptgen.py` & `linkml-1.7.9/linkml/generators/typescriptgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/yamlgen.py` & `linkml-1.7.9/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/generators/yumlgen.py` & `linkml-1.7.9/linkml/generators/yumlgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def visit_schema(
         self,
         classes: Set[ClassDefinitionName] = None,
         directory: Optional[str] = None,
         diagram_name: Optional[str] = None,
         load_image: bool = True,
         **_,
-    ) -> None:
+    ) -> Optional[str]:
         if directory:
             os.makedirs(directory, exist_ok=True)
         if classes is not None:
             for cls in classes:
                 if cls not in self.schema.classes:
                     raise ValueError(f"Unknown class name: {cls}")
         self.box_generated = set()
@@ -102,15 +102,15 @@
                     resp = requests.get(f"https://yuml.me/{filename}", stream=True, timeout=REQUESTS_TIMEOUT)
                     with open(self.output_file_name, "wb") as f:
                         for chunk in resp.iter_content(chunk_size=2048):
                             f.write(chunk)
                 else:
                     self.logger.error(f"{resp.reason} accessing {url}: {resp!r}")
         else:
-            print(str(YUML) + ",".join(yumlclassdef), end="")
+            return str(YUML) + ",".join(yumlclassdef)
 
     def class_box(self, cn: ClassDefinitionName) -> str:
         """Generate a box for the class.  Populate its interior only if (a) it hasn't previously been generated and
         (b) it appears in the gen_classes list
 
         @param cn:
         @return:
```

### Comparing `linkml-1.7.8/linkml/linter/cli.py` & `linkml-1.7.9/linkml/linter/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/config/datamodel/config.py` & `linkml-1.7.9/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/config/datamodel/config.yaml` & `linkml-1.7.9/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/config/default.yaml` & `linkml-1.7.9/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/formatters/formatter.py` & `linkml-1.7.9/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/formatters/json_formatter.py` & `linkml-1.7.9/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.7.9/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.7.9/linkml/linter/formatters/terminal_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.7.9/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/linter.py` & `linkml-1.7.9/linkml/linter/linter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/linter/rules.py` & `linkml-1.7.9/linkml/linter/rules.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/reporting/model.py` & `linkml-1.7.9/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/transformers/logical_model_transformer.py` & `linkml-1.7.9/linkml/transformers/logical_model_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/transformers/model_transformer.py` & `linkml-1.7.9/linkml/transformers/model_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/transformers/relmodel_transformer.py` & `linkml-1.7.9/linkml/transformers/relmodel_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/transformers/schema_renamer.py` & `linkml-1.7.9/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/cli_utils.py` & `linkml-1.7.9/linkml/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/converter.py` & `linkml-1.7.9/linkml/utils/converter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/datautils.py` & `linkml-1.7.9/linkml/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/execute_tutorial.py` & `linkml-1.7.9/linkml/utils/execute_tutorial.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/generator.py` & `linkml-1.7.9/linkml/utils/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,16 @@
 """
 
 import abc
 import logging
 import os
 import re
 import sys
-from contextlib import redirect_stdout
 from dataclasses import dataclass, field
 from functools import lru_cache
-from io import StringIO
 from pathlib import Path
 from typing import Callable, ClassVar, Dict, List, Mapping, Optional, Set, TextIO, Type, Union, cast
 
 import click
 from click import Argument, Command, Option
 from linkml_runtime import SchemaView
 from linkml_runtime.linkml_model.meta import (
@@ -172,14 +170,17 @@
 
     metamodel: SchemaLoader = None
     """A SchemaLoader instance that points to the LinkML metamodel (meta.yaml)"""
 
     stacktrace: bool = False
     """True means print stack trace, false just error message"""
 
+    include: Optional[Union[str, Path, SchemaDefinition]] = None
+    """If set, include extra schema outside of the imports mechanism"""
+
     def __post_init__(self) -> None:
         if not self.logger:
             self.logger = logging.getLogger()
         if self.log_level is not None:
             self.logger.setLevel(self.log_level)
         if self.format is None:
             self.format = self.valid_formats[0]
@@ -200,15 +201,20 @@
         # TODO: remove aliasing
         self.emit_metadata = self.metadata
         if self.uses_schemaloader:
             self._initialize_using_schemaloader(schema)
         else:
             logging.info(f"Using SchemaView with im={self.importmap} // base_dir={self.base_dir}")
             self.schemaview = SchemaView(schema, importmap=self.importmap, base_dir=self.base_dir)
+            if self.include:
+                if isinstance(self.include, (str, Path)):
+                    self.include = SchemaView(self.include, importmap=self.importmap, base_dir=self.base_dir).schema
+                self.schemaview.merge_schema(self.include)
             self.schema = self.schemaview.schema
+
         self._init_namespaces()
 
     def _initialize_using_schemaloader(self, schema: Union[str, TextIO, SchemaDefinition, "Generator"]):
         # currently generators are very liberal in what they accept, including
         # other generators.
         # See https://github.com/linkml/linkml/issues/923 for discussion on how
         # to simplify the overall framework
@@ -263,121 +269,137 @@
     def serialize(self, **kwargs) -> str:
         """
         Generate output in the required format
 
         :param kwargs: Generator specific parameters
         :return: Generated output
         """
-        output = StringIO()
-        # Note: we currently redirect stdout, this means that print statements within
-        # each generator will be redirected to the StringIO object.
-        # See https://github.com/linkml/linkml/issues/923 for discussion on simplifying this
-        with redirect_stdout(output):
-            # the default is to use the Visitor Pattern; each individual generator may
-            # choose to override methods {visit,end}_{element}.
-            # See https://github.com/linkml/linkml/issues/923
-            self.visit_schema(**kwargs)
-            for sn, ss in (
-                sorted(self.schema.subsets.items(), key=lambda s: s[0].lower())
-                if self.visits_are_sorted
-                else self.schema.subsets.items()
-            ):
-                self.visit_subset(ss)
-            for tn, typ in (
-                sorted(self.schema.types.items(), key=lambda s: s[0].lower())
-                if self.visits_are_sorted
-                else self.schema.types.items()
-            ):
-                self.visit_type(typ)
-            for enum in (
-                sorted(self.schema.enums.values(), key=lambda e: e.name.lower())
-                if self.visits_are_sorted
-                else self.schema.enums.values()
-            ):
-                self.visit_enum(enum)
-            for sn, slot in (
-                sorted(self.schema.slots.items(), key=lambda c: c[0].lower())
-                if self.visits_are_sorted
-                else self.schema.slots.items()
-            ):
-                self.visit_slot(self.aliased_slot_name(slot), slot)
-            for cls in (
-                sorted(self.schema.classes.values(), key=lambda c: c.name.lower())
-                if self.visits_are_sorted
-                else self.schema.classes.values()
-            ):
-                if self.visit_class(cls):
-                    for slot in self.all_slots(cls) if self.visit_all_class_slots else self.own_slots(cls):
-                        self.visit_class_slot(cls, self.aliased_slot_name(slot), slot)
-                    self.end_class(cls)
-            self.end_schema(**kwargs)
-        return output.getvalue()
+        out = ""
+
+        # the default is to use the Visitor Pattern; each individual generator may
+        # choose to override methods {visit,end}_{element}.
+        # See https://github.com/linkml/linkml/issues/923
+        sub_out = self.visit_schema(**kwargs)
+        if sub_out is not None:
+            out += sub_out
+        for sn, ss in (
+            sorted(self.schema.subsets.items(), key=lambda s: s[0].lower())
+            if self.visits_are_sorted
+            else self.schema.subsets.items()
+        ):
+            sub_out = self.visit_subset(ss)
+            if sub_out is not None:
+                out += sub_out
+        for tn, typ in (
+            sorted(self.schema.types.items(), key=lambda s: s[0].lower())
+            if self.visits_are_sorted
+            else self.schema.types.items()
+        ):
+            sub_out = self.visit_type(typ)
+            if sub_out is not None:
+                out += sub_out
+        for enum in (
+            sorted(self.schema.enums.values(), key=lambda e: e.name.lower())
+            if self.visits_are_sorted
+            else self.schema.enums.values()
+        ):
+            sub_out = self.visit_enum(enum)
+            if sub_out is not None:
+                out += sub_out
+        for sn, slot in (
+            sorted(self.schema.slots.items(), key=lambda c: c[0].lower())
+            if self.visits_are_sorted
+            else self.schema.slots.items()
+        ):
+            sub_out = self.visit_slot(self.aliased_slot_name(slot), slot)
+            if sub_out is not None:
+                out += sub_out
+        for cls in (
+            sorted(self.schema.classes.values(), key=lambda c: c.name.lower())
+            if self.visits_are_sorted
+            else self.schema.classes.values()
+        ):
+            cls_out = self.visit_class(cls)
+            if cls_out:
+                if isinstance(cls_out, str):
+                    out += cls_out
+                for slot in self.all_slots(cls) if self.visit_all_class_slots else self.own_slots(cls):
+                    sub_out = self.visit_class_slot(cls, self.aliased_slot_name(slot), slot)
+                    if sub_out is not None:
+                        out += sub_out
+                sub_out = self.end_class(cls)
+                if sub_out is not None:
+                    out += sub_out
+        sub_out = self.end_schema(**kwargs)
+        if sub_out is not None:
+            out += sub_out
+        return out
 
-    def visit_schema(self, **kwargs) -> None:
+    def visit_schema(self, **kwargs) -> Optional[str]:
         """Visited once at the beginning of generation
 
         @param kwargs: Arguments passed through from CLI -- implementation dependent
         """
         ...
 
-    def end_schema(self, **kwargs) -> None:
+    def end_schema(self, **kwargs) -> Optional[str]:
         """Visited once at the end of generation
 
         @param kwargs: Arguments passed through from CLI -- implementation dependent
         """
         ...
 
-    def visit_class(self, cls: ClassDefinition) -> bool:
+    def visit_class(self, cls: ClassDefinition) -> Optional[Union[str, bool]]:
         """Visited once per schema class
 
         @param cls: class being visited
         @return: Visit slots and end class.  False means skip and go on
         """
         return True
 
-    def end_class(self, cls: ClassDefinition) -> None:
+    def end_class(self, cls: ClassDefinition) -> Optional[str]:
         """Visited after visit_class_slots (if visit_class returned true)
 
         @param cls: class being visited
         """
         ...
 
-    def visit_class_slot(self, cls: ClassDefinition, aliased_slot_name: str, slot: SlotDefinition) -> None:
+    def visit_class_slot(self, cls: ClassDefinition, aliased_slot_name: str, slot: SlotDefinition) -> Optional[str]:
         """Visited for each slot in a class.  If class level visit_all_slots is true, this is visited once
         for any class that is inherited (class itself, is_a, mixin, apply_to).  Otherwise, just the own slots.
 
         @param cls: containing class
         @param aliased_slot_name: Aliased slot name.  May not be unique across all class slots
         @param slot: being visited
         """
         ...
 
-    def visit_slot(self, aliased_slot_name: str, slot: SlotDefinition) -> None:
+    def visit_slot(self, aliased_slot_name: str, slot: SlotDefinition) -> Optional[str]:
         """Visited once for every slot definition in the schema.
 
         @param aliased_slot_name: Aliased name of the slot.  May not be unique
         @param slot: visited slot
         """
         ...
 
-    def visit_type(self, typ: TypeDefinition) -> None:
+    def visit_type(self, typ: TypeDefinition) -> Optional[str]:
         """Visited once for every type definition in the schema
 
         @param typ: Type definition
         """
         ...
 
-    def visit_subset(self, subset: SubsetDefinition) -> None:
+    def visit_subset(self, subset: SubsetDefinition) -> Optional[str]:
         """Visited once for every subset definition in the schema
 
         #param subset: Subset definition
         """
         ...
 
-    def visit_enum(self, enum: EnumDefinition) -> None:
+    def visit_enum(self, enum: EnumDefinition) -> Optional[str]:
         """Visited once for every enum definition in the schema
 
         @param enum: Enum definition
         """
         ...
 
     # =============================
```

### Comparing `linkml-1.7.8/linkml/utils/ifabsent_functions.py` & `linkml-1.7.9/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/logictools.py` & `linkml-1.7.9/linkml/utils/logictools.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/mergeutils.py` & `linkml-1.7.9/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/rawloader.py` & `linkml-1.7.9/linkml/utils/rawloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/schema_builder.py` & `linkml-1.7.9/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/schema_fixer.py` & `linkml-1.7.9/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/schemaloader.py` & `linkml-1.7.9/linkml/utils/schemaloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/schemasynopsis.py` & `linkml-1.7.9/linkml/utils/schemasynopsis.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/sqlutils.py` & `linkml-1.7.9/linkml/utils/sqlutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/typereferences.py` & `linkml-1.7.9/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/utils/validation.py` & `linkml-1.7.9/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/__init__.py` & `linkml-1.7.9/linkml/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/cli.py` & `linkml-1.7.9/linkml/validator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,21 @@
 @click.option(
     "--include-range-class-descendants/--no-range-class-descendants",
     default=False,
     show_default=False,
     help=f"{DEPRECATED} When handling range constraints, include all descendants of the range "
     "class instead of just the range class",
 )
+@click.option(
+    "--include-context/--no-include-context",
+    "-D",
+    default=False,
+    show_default=True,
+    help="Include additional context when reporting of validation errors.",
+)
 @click.argument("data_sources", nargs=-1, type=click.Path(exists=True))
 @click.version_option(__version__, "-V", "--version")
 @click.pass_context
 def cli(
     context: click.Context,
     schema: Optional[Path],
     target_class: Optional[str],
@@ -119,14 +126,15 @@
     data_sources: Tuple[str],
     exit_on_first_failure: bool,
     legacy_mode: bool,
     module: Optional[str],
     input_format: Optional[str],
     index_slot: Optional[str],
     include_range_class_descendants: bool,
+    include_context: bool,
 ):
     if legacy_mode:
         from linkml.validators import jsonschemavalidator
 
         return context.invoke(
             jsonschemavalidator.cli,
             input=data_sources[0] if len(data_sources) > 0 else None,
@@ -179,14 +187,17 @@
     loaders = _resolve_loaders(config.data_sources)
     validator = Validator(config.schema_path, validation_plugins=plugins, strict=exit_on_first_failure)
     severity_counter = Counter()
     for loader in loaders:
         for result in validator.iter_results_from_source(loader, config.target_class):
             severity_counter[result.severity] += 1
             click.echo(f"[{result.severity.value}] [{loader.source}/{result.instance_index}] {result.message}")
+            if include_context:
+                for ctx in result.context:
+                    click.echo(f"[CONTEXT] {ctx}")
 
     if sum(severity_counter.values()) == 0:
         click.echo("No issues found")
 
     exit_code = 1 if severity_counter[Severity.ERROR] > 0 else 0
     sys.exit(exit_code)
```

### Comparing `linkml-1.7.8/linkml/validator/loaders/__init__.py` & `linkml-1.7.9/linkml/validator/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/loaders/delimited_file_loader.py` & `linkml-1.7.9/linkml/validator/loaders/delimited_file_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/loaders/json_loader.py` & `linkml-1.7.9/linkml/validator/loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/loaders/loader.py` & `linkml-1.7.9/linkml/validator/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/loaders/passthrough_loader.py` & `linkml-1.7.9/linkml/validator/loaders/passthrough_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/loaders/yaml_loader.py` & `linkml-1.7.9/linkml/validator/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/plugins/__init__.py` & `linkml-1.7.9/linkml/validator/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/plugins/jsonschema_validation_plugin.py` & `linkml-1.7.9/linkml/validator/plugins/jsonschema_validation_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         """
         validator = context.json_schema_validator(
             closed=self.closed,
             include_range_class_descendants=self.include_range_class_descendants,
             path_override=self.json_schema_path,
         )
         for error in validator.iter_errors(instance):
+            error_context = [ctx.message for ctx in error.context]
             best_error = best_match([error])
             yield ValidationResult(
                 type="jsonschema validation",
                 severity=Severity.ERROR,
                 instance=instance,
                 instantiates=context.target_class,
                 message=f"{best_error.message} in /{'/'.join(str(p) for p in best_error.absolute_path)}",
+                context=error_context,
             )
```

### Comparing `linkml-1.7.8/linkml/validator/plugins/pydantic_validation_plugin.py` & `linkml-1.7.9/linkml/validator/plugins/pydantic_validation_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/plugins/recommended_slots_plugin.py` & `linkml-1.7.9/linkml/validator/plugins/recommended_slots_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/plugins/shacl_validation_plugin.py` & `linkml-1.7.9/linkml/validator/plugins/shacl_validation_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/plugins/validation_plugin.py` & `linkml-1.7.9/linkml/validator/plugins/validation_plugin.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/report.py` & `linkml-1.7.9/linkml/validator/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     type: str
     severity: Severity
     message: str
     instance: Optional[Any] = None
     instance_index: Optional[int] = None
     instantiates: Optional[str] = None
+    context: List[str] = []
 
 
 class ValidationReport(BaseModel):
     """
     ValidationReport represents the result of all types of
     validation for a given object.
     A report object.
```

### Comparing `linkml-1.7.8/linkml/validator/validation_context.py` & `linkml-1.7.9/linkml/validator/validation_context.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validator/validator.py` & `linkml-1.7.9/linkml/validator/validator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validators/jsonschemavalidator.py` & `linkml-1.7.9/linkml/validators/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/validators/sparqlvalidator.py` & `linkml-1.7.9/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.7.9/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.7.9/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.7.8/linkml/workspaces/example_runner.py` & `linkml-1.7.9/linkml/workspaces/example_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import click
 import yaml
 from linkml_runtime import SchemaView
 from linkml_runtime.dumpers import json_dumper, rdflib_dumper, yaml_dumper
 from linkml_runtime.linkml_model import ElementName
 from linkml_runtime.utils.formatutils import camelcase
 
+from linkml._version import __version__
 from linkml.generators.pythongen import PythonGenerator
 from linkml.validator import Validator, _get_default_validator
 
 
 @dataclass
 class SummaryDocument:
     """
@@ -294,14 +295,15 @@
 )
 @click.option(
     "--use-type-designators/--no-use-type-designators",
     default=True,
     show_default=True,
     help="If true use type_designators to deepen ranges",
 )
+@click.version_option(__version__, "-V", "--version")
 def cli(schema, prefixes, output: TextIO, **kwargs):
     """Process a folder of examples and a folder of counter examples.
 
     Each example in the folder
 
     For context, see: https://github.com/linkml/linkml/issues/501
     """
```

### Comparing `linkml-1.7.8/pyproject.toml` & `linkml-1.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.7.8"
+version = "1.7.9"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
@@ -142,14 +142,15 @@
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.4.0"
 pytest-subtests = "^0.11.0"
 numpy = [
   { "version" = ">=1.24.3", "python" = "<3.12" },
   { "version" = ">=1.25.2", "python" = ">=3.12" }
 ]
+requests-cache = "^1.2.0"
 
 [tool.poetry.extras]
 black = ["black"]
 shacl = ["pyshacl"]
 tests = ["black", "pyshacl"]
 
 [tool.poetry.group.docs]
@@ -158,14 +159,16 @@
 [tool.poetry.group.docs.dependencies]
 furo = {version = "^2023.03.27", extras = ["docs"]}
 sphinxcontrib-mermaid = {version = "^0.7.1", extras = ["docs"]}
 sphinx = "*"
 sphinx-click = "*"
 sphinx-rtd-theme = "*"
 myst-parser = "*"
+matplotlib = ">=3.7"
+sphinx-jinja = "^2.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.codespell]
 # TODO: bring in tests in too
```

### Comparing `linkml-1.7.8/setup.py` & `linkml-1.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                      'linkml.validators.sparqlvalidator:cli',
                      'linkml-sqldb = linkml.utils.sqlutils:main',
                      'linkml-validate = linkml.validator.cli:cli',
                      'run-tutorial = linkml.utils.execute_tutorial:cli']}
 
 setup_kwargs = {
     'name': 'linkml',
-    'version': '1.7.8',
+    'version': '1.7.9',
     'description': 'Linked Open Data Modeling Language',
     'long_description': '[![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)\n![](https://github.com/linkml/linkml/workflows/Build/badge.svg)\n[![PyPi](https://img.shields.io/pypi/v/linkml.svg)](https://pypi.python.org/pypi/linkml)\n[![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml/main?filepath=notebooks)\n[![DOI](https://zenodo.org/badge/13996/linkml/linkml.svg)](https://zenodo.org/badge/latestdoi/13996/linkml/linkml)\n[![PyPIDownloadsTotal](https://pepy.tech/badge/linkml)](https://pepy.tech/project/linkml)\n[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml?logo=PyPI&color=blue)](https://pypi.org/project/linkml)\n[![codecov](https://codecov.io/gh/linkml/linkml/branch/main/graph/badge.svg?token=WNQNG986UN)](https://codecov.io/gh/linkml/linkml)\n\n\n# LinkML - Linked Data Modeling Language\n\nLinkML is a linked data modeling language following object-oriented and ontological principles. LinkML models are typically authored in YAML, and can be converted to other schema representation formats such as JSON or RDF.\n\nThis repo holds the tools for generating and working with LinkML. For the LinkML schema (metamodel), please see https://github.com/linkml/linkml-model\n\nThe complete documentation for LinkML can be found here:\n\n - [linkml.io/linkml](https://linkml.io/linkml)\n',
     'author': 'Chris Mungall',
     'author_email': 'cjmungall@lbl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://linkml.io/linkml/',
```

### Comparing `linkml-1.7.8/PKG-INFO` & `linkml-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.7.8
+Version: 1.7.9
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

