# Comparing `tmp/pylodstorage-0.9.1.tar.gz` & `tmp/pylodstorage-0.9.2.tar.gz`

## Comparing `pylodstorage-0.9.1.tar` & `pylodstorage-0.9.2.tar`

### file list

```diff
@@ -1,152 +1,152 @@
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/.pydevproject
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/.readthedocs.yml
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/.travis.yml
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/Makefile
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/conf.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/index.rst
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/lodstorage.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/make.bat
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/sampledata.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/setup.rst
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/tests.rst
--rw-r--r--   0        0        0  1971042 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/doctrees/index.doctree
--rw-r--r--   0        0        0  1108500 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/doctrees/lodstorage.doctree
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/doctrees/sampledata.doctree
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/doctrees/setup.doctree
--rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/doctrees/tests.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/.buildinfo
--rw-r--r--   0        0        0    60139 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/genindex.html
--rw-r--r--   0        0        0    82681 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/index.html
--rw-r--r--   0        0        0   463974 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/lodstorage.html
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/objects.inv
--rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/py-modindex.html
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/sampledata.html
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/search.html
--rw-r--r--   0        0        0    72544 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/searchindex.js
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/setup.html
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/tests.html
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/index.html
--rw-r--r--   0        0        0    21035 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/csv.html
--rw-r--r--   0        0        0    10645 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/docstring_parser.html
--rw-r--r--   0        0        0    71523 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/entity.html
--rw-r--r--   0        0        0    96049 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/jsonable.html
--rw-r--r--   0        0        0    12606 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/jsonpicklemixin.html
--rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/linkml.html
--rw-r--r--   0        0        0    26628 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/linkml_gen.html
--rw-r--r--   0        0        0    29264 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/lod.html
--rw-r--r--   0        0        0    16378 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/mwTable.html
--rw-r--r--   0        0        0    16814 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/plot.html
--rw-r--r--   0        0        0    98919 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/query.html
--rw-r--r--   0        0        0    50328 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/querymain.html
--rw-r--r--   0        0        0    24635 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/rdf.html
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sample.html
--rw-r--r--   0        0        0    28157 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sample2.html
--rw-r--r--   0        0        0    18430 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/schema.html
--rw-r--r--   0        0        0    73894 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sparql.html
--rw-r--r--   0        0        0    84441 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sql.html
--rw-r--r--   0        0        0    16704 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/storageconfig.html
--rw-r--r--   0        0        0    32202 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sync.html
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/tabulateCounter.html
--rw-r--r--   0        0        0   121135 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/trulytabular.html
--rw-r--r--   0        0        0    26618 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/uml.html
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/version.html
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/xml.html
--rw-r--r--   0        0        0    42606 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/yamlable.html
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/yamlablemixin.html
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_sources/lodstorage.rst.txt
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_sources/sampledata.rst.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_sources/setup.rst.txt
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_sources/tests.rst.txt
--rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/docs/source/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/__init__.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/cache.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/csv.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/docstring_parser.py
--rw-r--r--   0        0        0    17887 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/entity.py
--rw-r--r--   0        0        0    24517 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/jsonable.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/jsonpicklemixin.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/linkml.py
--rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/linkml_gen.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/lod.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/mwTable.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/plot.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/prefixes.py
--rw-r--r--   0        0        0    23699 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/query.py
--rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/querymain.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/rdf.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/sample.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/sample2.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/schema.py
--rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/sparql.py
--rw-r--r--   0        0        0    21959 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/sql.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/storageconfig.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/sync.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/tabulateCounter.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/uml.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/version.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/xml.py
--rw-r--r--   0        0        0    11014 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/yamlable.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/lodstorage/yamlablemixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/dblp.yaml
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/endpoints.yaml
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/example.ttl
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/formats.yaml
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/got.yaml
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/queries.yaml
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/royals.yaml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/royals_linkml_schema.yaml
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/scholia.yaml
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/trulytabular.yaml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/wf.yaml
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/sampledata/wikidata.yaml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/blackisort
--rwxr-xr-x   0        0        0     2192 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/doc
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/install
--rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/installAndTest
--rwxr-xr-x   0        0        0     5093 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/jena
--rwxr-xr-x   0        0        0     4875 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/sparqlquery
--rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/test
--rwxr-xr-x   0        0        0     2227 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/scripts/vsenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/basetest.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/testEntityManager.py
--rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/testJson.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/testPandas.py
--rw-r--r--   0        0        0    15959 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/testSPARQL.py
--rw-r--r--   0        0        0    15899 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/testSqlite3.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_Plot.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_cache.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_csv.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_docstring_parser.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_linkml.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_linkml_schema.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_lod.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_prefixes.py
--rw-r--r--   0        0        0    17564 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_queries.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_rdf.py
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_samples.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_sync.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_tabulate.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/tests/test_yamlable.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/LICENSE
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/README.md
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 pylodstorage-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/.pydevproject
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/.readthedocs.yml
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/.travis.yml
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/Makefile
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/conf.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/index.rst
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/lodstorage.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/make.bat
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/sampledata.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/setup.rst
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/tests.rst
+-rw-r--r--   0        0        0  1971042 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0  1108500 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/doctrees/lodstorage.doctree
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/doctrees/sampledata.doctree
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/doctrees/setup.doctree
+-rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/doctrees/tests.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/.buildinfo
+-rw-r--r--   0        0        0    60139 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/genindex.html
+-rw-r--r--   0        0        0    82681 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/index.html
+-rw-r--r--   0        0        0   463974 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/lodstorage.html
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/objects.inv
+-rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/py-modindex.html
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/sampledata.html
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/search.html
+-rw-r--r--   0        0        0    72544 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/searchindex.js
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/setup.html
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/tests.html
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/index.html
+-rw-r--r--   0        0        0    21035 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/csv.html
+-rw-r--r--   0        0        0    10645 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/docstring_parser.html
+-rw-r--r--   0        0        0    71523 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/entity.html
+-rw-r--r--   0        0        0    96049 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/jsonable.html
+-rw-r--r--   0        0        0    12606 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/jsonpicklemixin.html
+-rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/linkml.html
+-rw-r--r--   0        0        0    26628 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/linkml_gen.html
+-rw-r--r--   0        0        0    29264 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/lod.html
+-rw-r--r--   0        0        0    16378 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/mwTable.html
+-rw-r--r--   0        0        0    16814 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/plot.html
+-rw-r--r--   0        0        0    98919 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/query.html
+-rw-r--r--   0        0        0    50328 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/querymain.html
+-rw-r--r--   0        0        0    24635 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/rdf.html
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sample.html
+-rw-r--r--   0        0        0    28157 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sample2.html
+-rw-r--r--   0        0        0    18430 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/schema.html
+-rw-r--r--   0        0        0    73894 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sparql.html
+-rw-r--r--   0        0        0    84441 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sql.html
+-rw-r--r--   0        0        0    16704 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/storageconfig.html
+-rw-r--r--   0        0        0    32202 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sync.html
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/tabulateCounter.html
+-rw-r--r--   0        0        0   121135 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/trulytabular.html
+-rw-r--r--   0        0        0    26618 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/uml.html
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/version.html
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/xml.html
+-rw-r--r--   0        0        0    42606 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/yamlable.html
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/yamlablemixin.html
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_sources/lodstorage.rst.txt
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_sources/sampledata.rst.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_sources/setup.rst.txt
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_sources/tests.rst.txt
+-rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/docs/source/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/__init__.py
+-rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/cache.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/csv.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/docstring_parser.py
+-rw-r--r--   0        0        0    17887 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/entity.py
+-rw-r--r--   0        0        0    24517 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/jsonable.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/jsonpicklemixin.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/linkml.py
+-rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/linkml_gen.py
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/lod.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/mwTable.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/plot.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/prefixes.py
+-rw-r--r--   0        0        0    23699 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/query.py
+-rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/querymain.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/rdf.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/sample.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/sample2.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/schema.py
+-rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/sparql.py
+-rw-r--r--   0        0        0    21959 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/sql.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/storageconfig.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/sync.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/tabulateCounter.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/uml.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/version.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/xml.py
+-rw-r--r--   0        0        0    11014 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/yamlable.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/lodstorage/yamlablemixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/dblp.yaml
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/endpoints.yaml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/example.ttl
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/formats.yaml
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/got.yaml
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/queries.yaml
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/royals.yaml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/royals_linkml_schema.yaml
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/scholia.yaml
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/trulytabular.yaml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/wf.yaml
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/sampledata/wikidata.yaml
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/blackisort
+-rwxr-xr-x   0        0        0     2192 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/doc
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/install
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/installAndTest
+-rwxr-xr-x   0        0        0     5093 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/jena
+-rwxr-xr-x   0        0        0     4875 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/sparqlquery
+-rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/test
+-rwxr-xr-x   0        0        0     2227 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/scripts/vsenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/basetest.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/testEntityManager.py
+-rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/testJson.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/testPandas.py
+-rw-r--r--   0        0        0    15959 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/testSPARQL.py
+-rw-r--r--   0        0        0    15899 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/testSqlite3.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_Plot.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_cache.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_csv.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_docstring_parser.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_linkml.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_linkml_schema.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_lod.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_prefixes.py
+-rw-r--r--   0        0        0    17564 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_queries.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_rdf.py
+-rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_samples.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_sync.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_tabulate.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/tests/test_yamlable.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/README.md
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 pylodstorage-0.9.2/PKG-INFO
```

### Comparing `pylodstorage-0.9.1/.readthedocs.yml` & `pylodstorage-0.9.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/.github/workflows/build.yml` & `pylodstorage-0.9.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/.github/workflows/upload-to-pypi.yml` & `pylodstorage-0.9.2/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/Makefile` & `pylodstorage-0.9.2/docs/source/Makefile`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/conf.py` & `pylodstorage-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/lodstorage.rst` & `pylodstorage-0.9.2/docs/source/lodstorage.rst`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/make.bat` & `pylodstorage-0.9.2/docs/source/make.bat`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/tests.rst` & `pylodstorage-0.9.2/docs/source/tests.rst`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/doctrees/environment.pickle` & `pylodstorage-0.9.2/docs/source/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/doctrees/index.doctree` & `pylodstorage-0.9.2/docs/source/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/doctrees/lodstorage.doctree` & `pylodstorage-0.9.2/docs/source/_build/doctrees/lodstorage.doctree`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/doctrees/sampledata.doctree` & `pylodstorage-0.9.2/docs/source/_build/doctrees/sampledata.doctree`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/doctrees/setup.doctree` & `pylodstorage-0.9.2/docs/source/_build/doctrees/setup.doctree`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/doctrees/tests.doctree` & `pylodstorage-0.9.2/docs/source/_build/doctrees/tests.doctree`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/genindex.html` & `pylodstorage-0.9.2/docs/source/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/index.html` & `pylodstorage-0.9.2/docs/source/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/lodstorage.html` & `pylodstorage-0.9.2/docs/source/_build/html/lodstorage.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/objects.inv` & `pylodstorage-0.9.2/docs/source/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/py-modindex.html` & `pylodstorage-0.9.2/docs/source/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/sampledata.html` & `pylodstorage-0.9.2/docs/source/_build/html/sampledata.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/search.html` & `pylodstorage-0.9.2/docs/source/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/searchindex.js` & `pylodstorage-0.9.2/docs/source/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/setup.html` & `pylodstorage-0.9.2/docs/source/_build/html/setup.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/tests.html` & `pylodstorage-0.9.2/docs/source/_build/html/tests.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/index.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/csv.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/csv.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/docstring_parser.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/docstring_parser.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/entity.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/entity.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/jsonable.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/jsonable.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/jsonpicklemixin.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/jsonpicklemixin.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/linkml.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/linkml.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/linkml_gen.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/linkml_gen.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/lod.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/lod.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/mwTable.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/mwTable.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/plot.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/plot.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/query.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/query.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/querymain.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/querymain.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/rdf.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/rdf.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sample.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sample.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sample2.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sample2.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/schema.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/schema.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sparql.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sparql.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sql.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sql.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/storageconfig.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/storageconfig.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/sync.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/sync.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/tabulateCounter.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/tabulateCounter.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/trulytabular.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/trulytabular.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/uml.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/uml.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/version.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/version.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/xml.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/xml.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/yamlable.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/yamlable.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_modules/lodstorage/yamlablemixin.html` & `pylodstorage-0.9.2/docs/source/_build/html/_modules/lodstorage/yamlablemixin.html`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_sources/lodstorage.rst.txt` & `pylodstorage-0.9.2/docs/source/_build/html/_sources/lodstorage.rst.txt`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_sources/tests.rst.txt` & `pylodstorage-0.9.2/docs/source/_build/html/_sources/tests.rst.txt`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_static/alabaster.css` & `pylodstorage-0.9.2/docs/source/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_static/basic.css` & `pylodstorage-0.9.2/docs/source/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_static/doctools.js` & `pylodstorage-0.9.2/docs/source/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_static/language_data.js` & `pylodstorage-0.9.2/docs/source/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_static/pygments.css` & `pylodstorage-0.9.2/docs/source/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_static/searchtools.js` & `pylodstorage-0.9.2/docs/source/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/docs/source/_build/html/_static/sphinx_highlight.js` & `pylodstorage-0.9.2/docs/source/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/cache.py` & `pylodstorage-0.9.2/lodstorage/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,24 @@
         last_accessed: Optional; the last accessed timestamp of the cache.
     """
     name: str
     extension: str
     count_attr: str = None
     count: Optional[int] = None   
     
-    def set_path(self,base_path):
+    def set_path(self,base_path:str):
         """
-        set my path
+        Set my path based on the given base_path and ensure the parent directory is created.
+        
+        Args:
+            base_path (str): The base path where the directory should be created.
         """
         self.path = Path(f"{base_path}/{self.name}{self.extension}")
+        # Ensure parent directory is created
+        self.path.parent.mkdir(parents=True, exist_ok=True)
     
     @property
     def is_stored(self) -> bool:
         """Determines if the cache file exists and is not empty."""
         return self.path.is_file() and self.path.stat().st_size > 1
 
     @property
```

### Comparing `pylodstorage-0.9.1/lodstorage/csv.py` & `pylodstorage-0.9.2/lodstorage/csv.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/docstring_parser.py` & `pylodstorage-0.9.2/lodstorage/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/entity.py` & `pylodstorage-0.9.2/lodstorage/entity.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/jsonable.py` & `pylodstorage-0.9.2/lodstorage/jsonable.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/jsonpicklemixin.py` & `pylodstorage-0.9.2/lodstorage/jsonpicklemixin.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/linkml.py` & `pylodstorage-0.9.2/lodstorage/linkml.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/linkml_gen.py` & `pylodstorage-0.9.2/lodstorage/linkml_gen.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/lod.py` & `pylodstorage-0.9.2/lodstorage/lod.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/mwTable.py` & `pylodstorage-0.9.2/lodstorage/mwTable.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/plot.py` & `pylodstorage-0.9.2/lodstorage/plot.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/prefixes.py` & `pylodstorage-0.9.2/lodstorage/prefixes.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/query.py` & `pylodstorage-0.9.2/lodstorage/query.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/querymain.py` & `pylodstorage-0.9.2/lodstorage/querymain.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/rdf.py` & `pylodstorage-0.9.2/lodstorage/rdf.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/sample.py` & `pylodstorage-0.9.2/lodstorage/sample.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/sample2.py` & `pylodstorage-0.9.2/lodstorage/sample2.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/schema.py` & `pylodstorage-0.9.2/lodstorage/schema.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/sparql.py` & `pylodstorage-0.9.2/lodstorage/sparql.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/sql.py` & `pylodstorage-0.9.2/lodstorage/sql.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/storageconfig.py` & `pylodstorage-0.9.2/lodstorage/storageconfig.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/sync.py` & `pylodstorage-0.9.2/lodstorage/sync.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/tabulateCounter.py` & `pylodstorage-0.9.2/lodstorage/tabulateCounter.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/uml.py` & `pylodstorage-0.9.2/lodstorage/uml.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/xml.py` & `pylodstorage-0.9.2/lodstorage/xml.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/yamlable.py` & `pylodstorage-0.9.2/lodstorage/yamlable.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/lodstorage/yamlablemixin.py` & `pylodstorage-0.9.2/lodstorage/yamlablemixin.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/endpoints.yaml` & `pylodstorage-0.9.2/sampledata/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/example.ttl` & `pylodstorage-0.9.2/sampledata/example.ttl`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/got.yaml` & `pylodstorage-0.9.2/sampledata/got.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/queries.yaml` & `pylodstorage-0.9.2/sampledata/queries.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/royals.yaml` & `pylodstorage-0.9.2/sampledata/royals.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/royals_linkml_schema.yaml` & `pylodstorage-0.9.2/sampledata/royals_linkml_schema.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/scholia.yaml` & `pylodstorage-0.9.2/sampledata/scholia.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/trulytabular.yaml` & `pylodstorage-0.9.2/sampledata/trulytabular.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/wf.yaml` & `pylodstorage-0.9.2/sampledata/wf.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/sampledata/wikidata.yaml` & `pylodstorage-0.9.2/sampledata/wikidata.yaml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/scripts/doc` & `pylodstorage-0.9.2/scripts/doc`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/scripts/jena` & `pylodstorage-0.9.2/scripts/jena`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/scripts/sparqlquery` & `pylodstorage-0.9.2/scripts/sparqlquery`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/scripts/vsenv` & `pylodstorage-0.9.2/scripts/vsenv`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/basetest.py` & `pylodstorage-0.9.2/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/testEntityManager.py` & `pylodstorage-0.9.2/tests/testEntityManager.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/testJson.py` & `pylodstorage-0.9.2/tests/testJson.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/testPandas.py` & `pylodstorage-0.9.2/tests/testPandas.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/testSPARQL.py` & `pylodstorage-0.9.2/tests/testSPARQL.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/testSqlite3.py` & `pylodstorage-0.9.2/tests/testSqlite3.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_Plot.py` & `pylodstorage-0.9.2/tests/test_Plot.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_cache.py` & `pylodstorage-0.9.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_csv.py` & `pylodstorage-0.9.2/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_docstring_parser.py` & `pylodstorage-0.9.2/tests/test_docstring_parser.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_linkml.py` & `pylodstorage-0.9.2/tests/test_linkml.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_linkml_schema.py` & `pylodstorage-0.9.2/tests/test_linkml_schema.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_lod.py` & `pylodstorage-0.9.2/tests/test_lod.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_prefixes.py` & `pylodstorage-0.9.2/tests/test_prefixes.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_queries.py` & `pylodstorage-0.9.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_rdf.py` & `pylodstorage-0.9.2/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_samples.py` & `pylodstorage-0.9.2/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_sync.py` & `pylodstorage-0.9.2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_tabulate.py` & `pylodstorage-0.9.2/tests/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/tests/test_yamlable.py` & `pylodstorage-0.9.2/tests/test_yamlable.py`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/.gitignore` & `pylodstorage-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/LICENSE` & `pylodstorage-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/README.md` & `pylodstorage-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/pyproject.toml` & `pylodstorage-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylodstorage-0.9.1/PKG-INFO` & `pylodstorage-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLodStorage
-Version: 0.9.1
+Version: 0.9.2
 Project-URL: Home, https://github.com/WolfgangFahl/pyLodStorage
 Project-URL: Documentation, http://wiki.bitplan.com/index.php/PyLoDStorage
 Project-URL: Source, https://github.com/WolfgangFahl/pyLodStorage/blob/master/lodstorage/sql.py
 Project-URL: IssueTracker, https://github.com/WolfgangFahl/pyLodStorage/issues
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
```

