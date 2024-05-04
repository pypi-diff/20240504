# Comparing `tmp/histcite-python-1.1.0.tar.gz` & `tmp/histcite_python-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-1.1.0.tar", last modified: Sun Mar  3 14:20:06 2024, max compression
+gzip compressed data, was "histcite_python-2.0.0.tar", last modified: Sat May  4 18:29:09 2024, max compression
```

## Comparing `histcite-python-1.1.0.tar` & `histcite_python-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:20:06.219425 histcite-python-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-03 14:19:57.000000 histcite-python-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-03-03 14:20:06.219425 histcite-python-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-03-03 14:19:57.000000 histcite-python-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:20:06.219425 histcite-python-1.1.0/histcite/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/parse_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/process_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/read_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-03 14:19:57.000000 histcite-python-1.1.0/histcite/recognize_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:20:06.219425 histcite-python-1.1.0/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-03-03 14:20:06.000000 histcite-python-1.1.0/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-03 14:20:06.000000 histcite-python-1.1.0/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 14:20:06.000000 histcite-python-1.1.0/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-03 14:20:06.000000 histcite-python-1.1.0/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-03 14:20:06.000000 histcite-python-1.1.0/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-03 14:20:06.000000 histcite-python-1.1.0/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-03 14:19:57.000000 histcite-python-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 14:20:06.219425 histcite-python-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:20:06.219425 histcite-python-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-03 14:19:57.000000 histcite-python-1.1.0/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-03 14:19:57.000000 histcite-python-1.1.0/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-03 14:19:57.000000 histcite-python-1.1.0/tests/test_parse_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-03 14:19:57.000000 histcite-python-1.1.0/tests/test_process_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-03 14:19:57.000000 histcite-python-1.1.0/tests/test_read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:29:09.244504 histcite_python-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 18:29:01.000000 histcite_python-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-04 18:29:09.244504 histcite_python-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-04 18:29:01.000000 histcite_python-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:29:09.240504 histcite_python-2.0.0/histcite/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-04 18:29:01.000000 histcite_python-2.0.0/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-04 18:29:01.000000 histcite_python-2.0.0/histcite/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-04 18:29:01.000000 histcite_python-2.0.0/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-04 18:29:01.000000 histcite_python-2.0.0/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-04 18:29:01.000000 histcite_python-2.0.0/histcite/parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-04 18:29:01.000000 histcite_python-2.0.0/histcite/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-05-04 18:29:01.000000 histcite_python-2.0.0/histcite/read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:29:09.244504 histcite_python-2.0.0/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-04 18:29:09.000000 histcite_python-2.0.0/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-04 18:29:09.000000 histcite_python-2.0.0/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:29:09.000000 histcite_python-2.0.0/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 18:29:09.000000 histcite_python-2.0.0/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 18:29:09.000000 histcite_python-2.0.0/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 18:29:09.000000 histcite_python-2.0.0/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-04 18:29:01.000000 histcite_python-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:29:09.244504 histcite_python-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:29:09.244504 histcite_python-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:29:01.000000 histcite_python-2.0.0/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:29:01.000000 histcite_python-2.0.0/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-04 18:29:01.000000 histcite_python-2.0.0/tests/test_parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:29:01.000000 histcite_python-2.0.0/tests/test_process_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-04 18:29:01.000000 histcite_python-2.0.0/tests/test_read_file.py
```

### Comparing `histcite-python-1.1.0/LICENSE` & `histcite_python-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-1.1.0/PKG-INFO` & `histcite_python-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 1.1.0
+Version: 2.0.0
 Summary: A Python interface for histcite
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/doublessay/histcite-python
 Keywords: histcite,citation network,web of science,scopus,cssci
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -20,58 +20,58 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=2.0
 Requires-Dist: pyarrow
 Requires-Dist: openpyxl
+Requires-Dist: refparse
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
-# HistCite工具的Python实现
+# HistCite 工具的 Python 实现
 
 [![PyPI](https://img.shields.io/pypi/v/histcite-python)](https://pypi.org/project/histcite-python)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/histcite-python.svg)](https://pypi.org/project/histcite-python)
 [![Codecov](https://codecov.io/gh/doublessay/histcite-python/graph/badge.svg?token=99V9E2CI1H)](https://codecov.io/gh/doublessay/histcite-python)
 [![License](https://img.shields.io/pypi/l/histcite-python.svg)](https://github.com/doublessay/histcite-python/blob/main/LICENSE)
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内使用较多的为中科大某同学 (知乎昵称[Tsing](https://www.zhihu.com/people/wq123)) 在源程序基础上修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅适用于 `Windows` 平台，存在较大限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具实现了 `HistCite` 的核心功能，可以跨平台使用，同时拓展了对 [其他数据源](#数据准备) 的支持。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内使用较多的为中科大某同学 (知乎昵称 [Tsing](https://www.zhihu.com/people/wq123)) 在源程序基础上修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅适用于 `Windows` 平台，存在较大限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具实现了 `HistCite` 的核心功能，可以跨平台使用，同时拓展了对 [其他数据源](#数据准备) 的支持。
 
 核心功能：
 - 生成引文网络图；
 - 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
-- 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 工具对比：
 |对比项|histcite-python|histcite pro|
 |:----|:----|:----|
 |是否开源|是|否|
 |是否跨平台|是|否，仅限 Windows|
 |是否支持其他数据源|是|否，仅限 Web of Science|
-|是否提供前端界面|否|是|
+|是否提供前端界面|否|是，可交互|
 |引文网络图|矢量图，比较清晰|位图，比较模糊|
 
 ## 快速开始
 ```console
-pip install histcite-python
+$ pip install histcite-python
 ```
 
 ## 数据准备
 |数据来源|下载说明|原始文件名|
 |:----|:----|:----|
 |Web of Science|`核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custom selection/自定义选择项`，全选字段。|`savedrecs*.txt`|
 |CSSCI|从 `CSSCI数据库` 正常导出即可。|`LY_*.txt`|
-|Scopus|格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。|`scopus*.csv`|
+|Scopus|网站语言切换到英文，格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。|`scopus*.csv`|
 
 > [!WARNING]
-> 文件下载后不要重命名(会根据文件名识别有效的题录数据文件)，把下载的所有文件放在一个单独的文件夹内。
+> 文件下载后不要重命名(会根据文件名识别有效的数据文件)，把下载的所有文件放在一个单独的文件夹内。
 
 ## 使用方法
 1. 使用命令行工具
 ```console
 $ histcite -h
 usage: histcite [-h] (--top TOP | --threshold THRESHOLD | --node NODE) [--disable_timeline] folder_path {wos,cssci,scopus}
 
@@ -85,80 +85,74 @@
   -h, --help            show this help message and exit
   --top                 Top N nodes with the highest LCS.
   --threshold           Nodes with LCS greater than threshold.
   --disable_timeline    Whether to disable timeline.
 ```
 
 ```console
-$ histcite /Users/.../Downloads/dataset wos --top 100 --disable_timeline
+$ histcite /Users/.../Downloads/dataset wos --top 50 --disable_timeline
 ```
 
 > [!NOTE]
 > 生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含
-> - 描述统计表 descriptive_statistics.xlsx
 > - 引文网络图节点信息表 graph_node_info.xlsx
 > - 引文网络图的数据文件 graph.dot
->     - 借助 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+>     - 借助 [Graphviz 在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz](https://graphviz.org/) 生成引文网络图。
 
 引文网络图示例：
 
 ![](https://raw.githubusercontent.com/doublessay/histcite-python/main/examples/graph.svg)
 
-对应的节点信息如下(以CSSCI数据源为例，不同文献数据库的节点信息字段存在差异)：
+对应的节点信息如下(以 CSSCI 数据源为例)：
 | |AU|TI|PY|SO|LCS|
 |:----|:----|:----|:----|:----|:----|
 |55|张坤; 查先进|我国智慧图书馆的发展沿革及构建策略研究|2021|国家图书馆学刊|6|
 |60|石婷婷; 徐建华; 张雨浓|数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计|2021|情报理论与实践|7|
 |63|卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷|智慧图书馆建设标准探析|2021|中国图书馆学报|9|
 |81|程焕文; 钟远薪|智慧图书馆的三维解析|2021|图书馆论坛|10|
 |86|段美珍; 初景利; 张冬荣; 解贺嘉|智慧图书馆的内涵特点及其认知模型研究|2021|图书情报工作|7|
 |...| | | | | |
 
-2. 使用 Jupyter，比命令行更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+2. 使用 Jupyter Notebook，可以自定义更多参数，导出描述性统计数据，请查看 [demo.ipynb](demo.ipynb)
 
 ## 字段说明
 |Field Name|Description|
 |:----|:----|
 |`GCS`|Global Citation Score, 表示一篇文献在文献数据库中的总被引次数|
 |`LCS`|Local Citation Score, 表示一篇文献在本地文献集中的被引次数|
 |`GCR`|Global Cited References, 表示一篇文献的参考文献数量|
 |`LCR`|Local Cited References, 表示一篇文献的参考文献在本地文献集中的数量|
 |`T*` |Total score, e.g. TLCS = Total Local Citation Scores.|
 |`Recs`|Count of Records|
 |`FAU`|First Author|
 |`CAU`|Corresponding Authors|
 |`AU`|Authors|
-|`EM`|Email Address|
 |`CO`|Country of Authors|
 |`C1`|Addresses|
 |`C3`|Author Affiliations|
 |`RP`|Reprint Address|
 |`I2`|Institution with Subdivision|
 |`TI`|Article Title|
 |`SO`|Source Title|
 |`DT`|Document Type|
-|`FU`|Funding Orgs|
 |`DE`|Author Keywords|
 |`CR`|Cited References|
 |`NR`|Cited Reference Count|
 |`TC`|Times Cited Count|
-|`J9`|Journal Abbreviation|
 |`PY`|Publication Year|
 |`VL`|Volume|
 |`IS`|Issue|
 |`BP`|Start Page|
 |`EP`|End Page|
 |`DI`|DOI|
 |...|[Please refer to Web of Science fields.](https://webofscience.help.clarivate.com/en-us/Content/export-records.htm)|
 
 ## FAQ
 1. 为什么生成的引文网络图时间线会错乱？
-- Graphviz 会自动调整节点位置，节点数量较少时容易出现这一问题。可以通过设置参数来关闭时间线。
+- 节点位置由 Graphviz 自动调整，节点数量较少时容易出现这一问题。可以通过设置参数隐藏时间线。
 
-2. 想要分析其他来源的文献元数据？
-- 该数据源能够导出文献的参考文献或引文数据。如果满足这一条件的话，欢迎提交 [Feature Request](https://github.com/doublessay/histcite-python/issues)，我们会尽快支持。
-
-3. 是否存在其他类似的工具？
+2. 是否存在其他类似的工具？
 - [CiteSpace](https://citespace.podia.com/)
 - [CitNetExplorer](https://www.citnetexplorer.nl/)
+- [VOSviewer](https://www.vosviewer.com/)
 - [Connected Papers](https://www.connectedpapers.com/)
 - [Litmaps](https://app.litmaps.com/)
```

### Comparing `histcite-python-1.1.0/README.md` & `histcite_python-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-# HistCite工具的Python实现
+# HistCite 工具的 Python 实现
 
 [![PyPI](https://img.shields.io/pypi/v/histcite-python)](https://pypi.org/project/histcite-python)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/histcite-python.svg)](https://pypi.org/project/histcite-python)
 [![Codecov](https://codecov.io/gh/doublessay/histcite-python/graph/badge.svg?token=99V9E2CI1H)](https://codecov.io/gh/doublessay/histcite-python)
 [![License](https://img.shields.io/pypi/l/histcite-python.svg)](https://github.com/doublessay/histcite-python/blob/main/LICENSE)
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内使用较多的为中科大某同学 (知乎昵称[Tsing](https://www.zhihu.com/people/wq123)) 在源程序基础上修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅适用于 `Windows` 平台，存在较大限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具实现了 `HistCite` 的核心功能，可以跨平台使用，同时拓展了对 [其他数据源](#数据准备) 的支持。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内使用较多的为中科大某同学 (知乎昵称 [Tsing](https://www.zhihu.com/people/wq123)) 在源程序基础上修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅适用于 `Windows` 平台，存在较大限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具实现了 `HistCite` 的核心功能，可以跨平台使用，同时拓展了对 [其他数据源](#数据准备) 的支持。
 
 核心功能：
 - 生成引文网络图；
 - 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
-- 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 工具对比：
 |对比项|histcite-python|histcite pro|
 |:----|:----|:----|
 |是否开源|是|否|
 |是否跨平台|是|否，仅限 Windows|
 |是否支持其他数据源|是|否，仅限 Web of Science|
-|是否提供前端界面|否|是|
+|是否提供前端界面|否|是，可交互|
 |引文网络图|矢量图，比较清晰|位图，比较模糊|
 
 ## 快速开始
 ```console
-pip install histcite-python
+$ pip install histcite-python
 ```
 
 ## 数据准备
 |数据来源|下载说明|原始文件名|
 |:----|:----|:----|
 |Web of Science|`核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custom selection/自定义选择项`，全选字段。|`savedrecs*.txt`|
 |CSSCI|从 `CSSCI数据库` 正常导出即可。|`LY_*.txt`|
-|Scopus|格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。|`scopus*.csv`|
+|Scopus|网站语言切换到英文，格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。|`scopus*.csv`|
 
 > [!WARNING]
-> 文件下载后不要重命名(会根据文件名识别有效的题录数据文件)，把下载的所有文件放在一个单独的文件夹内。
+> 文件下载后不要重命名(会根据文件名识别有效的数据文件)，把下载的所有文件放在一个单独的文件夹内。
 
 ## 使用方法
 1. 使用命令行工具
 ```console
 $ histcite -h
 usage: histcite [-h] (--top TOP | --threshold THRESHOLD | --node NODE) [--disable_timeline] folder_path {wos,cssci,scopus}
 
@@ -52,80 +51,74 @@
   -h, --help            show this help message and exit
   --top                 Top N nodes with the highest LCS.
   --threshold           Nodes with LCS greater than threshold.
   --disable_timeline    Whether to disable timeline.
 ```
 
 ```console
-$ histcite /Users/.../Downloads/dataset wos --top 100 --disable_timeline
+$ histcite /Users/.../Downloads/dataset wos --top 50 --disable_timeline
 ```
 
 > [!NOTE]
 > 生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含
-> - 描述统计表 descriptive_statistics.xlsx
 > - 引文网络图节点信息表 graph_node_info.xlsx
 > - 引文网络图的数据文件 graph.dot
->     - 借助 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+>     - 借助 [Graphviz 在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz](https://graphviz.org/) 生成引文网络图。
 
 引文网络图示例：
 
 ![](https://raw.githubusercontent.com/doublessay/histcite-python/main/examples/graph.svg)
 
-对应的节点信息如下(以CSSCI数据源为例，不同文献数据库的节点信息字段存在差异)：
+对应的节点信息如下(以 CSSCI 数据源为例)：
 | |AU|TI|PY|SO|LCS|
 |:----|:----|:----|:----|:----|:----|
 |55|张坤; 查先进|我国智慧图书馆的发展沿革及构建策略研究|2021|国家图书馆学刊|6|
 |60|石婷婷; 徐建华; 张雨浓|数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计|2021|情报理论与实践|7|
 |63|卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷|智慧图书馆建设标准探析|2021|中国图书馆学报|9|
 |81|程焕文; 钟远薪|智慧图书馆的三维解析|2021|图书馆论坛|10|
 |86|段美珍; 初景利; 张冬荣; 解贺嘉|智慧图书馆的内涵特点及其认知模型研究|2021|图书情报工作|7|
 |...| | | | | |
 
-2. 使用 Jupyter，比命令行更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+2. 使用 Jupyter Notebook，可以自定义更多参数，导出描述性统计数据，请查看 [demo.ipynb](demo.ipynb)
 
 ## 字段说明
 |Field Name|Description|
 |:----|:----|
 |`GCS`|Global Citation Score, 表示一篇文献在文献数据库中的总被引次数|
 |`LCS`|Local Citation Score, 表示一篇文献在本地文献集中的被引次数|
 |`GCR`|Global Cited References, 表示一篇文献的参考文献数量|
 |`LCR`|Local Cited References, 表示一篇文献的参考文献在本地文献集中的数量|
 |`T*` |Total score, e.g. TLCS = Total Local Citation Scores.|
 |`Recs`|Count of Records|
 |`FAU`|First Author|
 |`CAU`|Corresponding Authors|
 |`AU`|Authors|
-|`EM`|Email Address|
 |`CO`|Country of Authors|
 |`C1`|Addresses|
 |`C3`|Author Affiliations|
 |`RP`|Reprint Address|
 |`I2`|Institution with Subdivision|
 |`TI`|Article Title|
 |`SO`|Source Title|
 |`DT`|Document Type|
-|`FU`|Funding Orgs|
 |`DE`|Author Keywords|
 |`CR`|Cited References|
 |`NR`|Cited Reference Count|
 |`TC`|Times Cited Count|
-|`J9`|Journal Abbreviation|
 |`PY`|Publication Year|
 |`VL`|Volume|
 |`IS`|Issue|
 |`BP`|Start Page|
 |`EP`|End Page|
 |`DI`|DOI|
 |...|[Please refer to Web of Science fields.](https://webofscience.help.clarivate.com/en-us/Content/export-records.htm)|
 
 ## FAQ
 1. 为什么生成的引文网络图时间线会错乱？
-- Graphviz 会自动调整节点位置，节点数量较少时容易出现这一问题。可以通过设置参数来关闭时间线。
+- 节点位置由 Graphviz 自动调整，节点数量较少时容易出现这一问题。可以通过设置参数隐藏时间线。
 
-2. 想要分析其他来源的文献元数据？
-- 该数据源能够导出文献的参考文献或引文数据。如果满足这一条件的话，欢迎提交 [Feature Request](https://github.com/doublessay/histcite-python/issues)，我们会尽快支持。
-
-3. 是否存在其他类似的工具？
+2. 是否存在其他类似的工具？
 - [CiteSpace](https://citespace.podia.com/)
 - [CitNetExplorer](https://www.citnetexplorer.nl/)
+- [VOSviewer](https://www.vosviewer.com/)
 - [Connected Papers](https://www.connectedpapers.com/)
 - [Litmaps](https://app.litmaps.com/)
```

### Comparing `histcite-python-1.1.0/histcite/__main__.py` & `histcite_python-2.0.0/histcite/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 from pathlib import Path
 
-from .compute_metrics import ComputeMetrics
 from .network_graph import GraphViz
-from .process_file import ProcessFile
+from .process_file import BuildCitation, BuildRef
 from .read_file import ReadFile
 
 
 def cli():
     parser = argparse.ArgumentParser(description="A Python interface for histcite.")
     # Positional arguments
     parser.add_argument(
@@ -39,35 +38,25 @@
 
     args = parser.parse_args()
     folder_path = Path(args.folder_path)
     output_path = folder_path / "result"
     Path.mkdir(output_path, exist_ok=True)
 
     docs_df = ReadFile(folder_path, args.source).read_all()
-    process = ProcessFile(docs_df, args.source)
-    refs_df = process.extract_reference()
-    citation_relation = process.process_citation(refs_df)
-
-    cm = ComputeMetrics(docs_df, citation_relation, args.source)
-    cm.write2excel(output_path / "descriptive_statistics.xlsx")
-
-    graph = GraphViz(docs_df, citation_relation, args.source)
+    refs_df = BuildRef(docs_df, args.source).build()
+    citation_matrix = BuildCitation(docs_df, refs_df, args.source).build()
 
+    graph = GraphViz(docs_df, citation_matrix, args.source)
     if args.top is not None:
-        doc_id_list = (
-            citation_relation[citation_relation["LCS"] > 0]
-            .sort_values("LCS", ascending=False)
-            .index[: args.top]
-            .tolist()
-        )
+        node_list = citation_matrix[citation_matrix["LCS"] > 0].sort_values("LCS", ascending=False).index[: args.top].tolist()
 
     elif args.threshold is not None:
-        doc_id_list = citation_relation[citation_relation["LCS"] >= args.threshold].index.tolist()
+        node_list = citation_matrix[citation_matrix["LCS"] >= args.threshold].index.tolist()
 
     else:
         raise ValueError("<top> or <threshold> must be specified.")
 
-    graph_dot_file = graph.generate_dot_file(doc_id_list, show_timeline=args.disable_timeline)
+    graph_dot_file = graph.generate_dot_file(node_list, show_timeline=args.disable_timeline)
     graph_dot_path = output_path / "graph.dot"
     with open(graph_dot_path, "w") as f:
         f.write(graph_dot_file)
     graph.export_graph_node_info(output_path / "graph_node_info.xlsx")
```

### Comparing `histcite-python-1.1.0/histcite/compute_metrics.py` & `histcite_python-2.0.0/histcite/compute_metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "Authors",
     "Journals",
     "Keywords",
     "Yearly output",
     "Document Type",
     "Institution",
     "Institution with Subdivision",
+    "Corresponding Authors",
     "Country",
 ]
 
 cssci_analyses_index = [
     "Records",
     "Authors",
     "Journals",
@@ -38,28 +39,21 @@
 
 class ComputeMetrics:
     """Compute descriptive statistics of docs."""
 
     def __init__(
         self,
         docs_df: pd.DataFrame,
-        citation_relation: pd.DataFrame,
+        citation_matrix: pd.DataFrame,
         source: Literal["wos", "cssci", "scopus"],
     ):
-        """
-        Args:
-            docs_df: DataFrame of docs.
-            citation_relation: DataFrame of citation relationship.
-            source: Data source. `wos`, `cssci` or `scopus`.
-        """
-        self.merged_docs_df: pd.DataFrame = docs_df.merge(citation_relation[["doc_id", "LCR", "LCS"]], on="doc_id")
-        self.source: Literal["wos", "cssci", "scopus"] = source
+        self.merged_docs_df = docs_df.merge(citation_matrix[["node", "LCR", "LCS"]], on="node")
+        self.source = source
 
-    def check_analyses_index(self) -> list[str]:
-        """Return the index of analyses."""
+    def check_sheets(self) -> list[str]:
         if self.source == "wos":
             return wos_analyses_index
         elif self.source == "cssci":
             return cssci_analyses_index
         elif self.source == "scopus":
             return scopus_analyses_index
         else:
@@ -81,146 +75,112 @@
             split_char: Whether to split string. e.g. `; `. Default None.
             lower_case: Whether to convert string to lowercase. Default False.
             sort_by_col: Sort DataFrame by column. `Recs`, `TLCS` or `TGCS`. Default `Recs`.
 
         Returns:
             A DataFrame with some statitical metrics.
         """
-        assert col in use_cols, "Argument <col> must be in use_cols"
+        assert col in use_cols, "Argument <col> must be in <use_cols>"
         if sort_by_col == "TLCS":
-            assert "LCS" in use_cols, "LCS must be in <use_cols> when sorting by TLCS"
+            assert "LCS" in use_cols
         elif sort_by_col == "TGCS":
-            assert "TC" in use_cols, "TC must be in <use_cols> when sorting by TGCS"
+            assert "TC" in use_cols
 
         df = self.merged_docs_df[use_cols].dropna(subset=[col])
         if lower_case:
             df[col] = df[col].str.lower()
         if split_char:
             df[col] = df[col].str.split(split_char)
-            df = df.explode(col)
-            df = df.reset_index(drop=True)
+            df = df.explode(col, ignore_index=True)
 
+        agg_dict = {col: "count"}
         if "LCS" in use_cols:
-            if "TC" in use_cols:
-                grouped_df = df.groupby(col).agg({col: "count", "LCS": "sum", "TC": "sum"})
-            else:
-                grouped_df = df.groupby(col).agg({col: "count", "LCS": "sum"})
-        else:
-            grouped_df = df.groupby(col).agg({col: "count"})
-
+            agg_dict.update({"LCS": "sum"})
+        if "TC" in use_cols:
+            agg_dict.update({"TC": "sum"})
+        grouped_df = df.groupby(col).agg(agg_dict)
         grouped_df.rename(columns={col: "Recs", "LCS": "TLCS", "TC": "TGCS"}, inplace=True)
-        # e.g. Andersson, Gerhard (7202645907)
-        if col == "Author full names":
-            grouped_df.index = grouped_df.index.str.replace(r" \(\d+\)", "", regex=True)
-
-        if not sort_by_col:
-            sort_by_col = "Recs"
         return grouped_df.sort_values(sort_by_col, ascending=False)
 
     def generate_record_df(self) -> pd.DataFrame:
         """Return record DataFrame."""
-        if self.source in ["wos", "scopus"]:
-            use_cols = [
-                "AU",
-                "TI",
-                "SO",
-                "PY",
-                "TI",
-                "LCS",
-                "TC",
-                "LCR",
-                "NR",
-                "source file",
-            ]
-        elif self.source == "cssci":
-            use_cols = ["AU", "TI", "SO", "PY", "LCS", "LCR", "NR", "source file"]
-        else:
-            raise ValueError("Invalid source type")
+        use_cols = [
+            "AU",
+            "TI",
+            "SO",
+            "PY",
+            "LCS",
+            "TC",
+            "LCR",
+            "NR",
+            "source file",
+        ]
+        if self.source == "cssci":
+            use_cols.remove("TC")
         records_df = self.merged_docs_df[use_cols]
         if "TC" in use_cols:
             records_df = records_df.rename(columns={"TC": "GCS"})
         if "NR" in use_cols:
             records_df = records_df.rename(columns={"NR": "GCR"})
         return records_df
 
     def generate_author_df(self) -> pd.DataFrame:
         """Return author DataFrame."""
-        if self.source == "wos":
-            use_cols = ["AU", "LCS", "TC"]
-        elif self.source == "cssci":
-            use_cols = ["AU", "LCS"]
-        elif self.source == "scopus":
-            use_cols = ["Author full names", "LCS", "TC"]
-        else:
-            raise ValueError("Invalid source type")
-        return self.generate_df_factory(use_cols, use_cols[0], "; ")
+        use_cols = ["AU", "LCS", "TC"]
+        if self.source == "cssci":
+            use_cols.remove("TC")
+        return self.generate_df_factory(use_cols, "AU", "; ")
 
     def generate_corresponding_author_df(self) -> pd.DataFrame:
-        """Return corresponding author DataFrame. Only support WOS."""
+        """Return corresponding author DataFrame. Only support WoS."""
         if self.source == "wos":
             use_cols = ["CAU", "LCS", "TC"]
-        else:
-            raise ValueError("Invalid source type")
         return self.generate_df_factory(use_cols, "CAU", "; ")
 
     def generate_keyword_df(self) -> pd.DataFrame:
         """Return keyword DataFrame."""
-        if self.source in ["wos", "scopus"]:
-            use_cols = ["DE", "LCS", "TC"]
-        elif self.source == "cssci":
-            use_cols = ["DE", "LCS"]
-        else:
-            raise ValueError("Invalid source type")
+        use_cols = ["DE", "LCS", "TC"]
+        if self.source == "cssci":
+            use_cols.remove("TC")
         return self.generate_df_factory(use_cols, "DE", "; ", True)
 
     def generate_institution_df(self) -> pd.DataFrame:
         """Return institution DataFrame. Not support Scopus."""
-        assert self.source != "scopus", "Scopus is not supported to analyze <institution> field yet."
         if self.source == "wos":
             use_cols = ["C3", "LCS", "TC"]
         elif self.source == "cssci":
             use_cols = ["C3", "LCS"]
-        else:
-            raise ValueError("Invalid source type")
         return self.generate_df_factory(use_cols, "C3", "; ")
 
-    def generate_i2_df(self) -> pd.DataFrame:
+    def generate_sub_institution_df(self) -> pd.DataFrame:
         """Return institution with subdivision DataFrame. Only support WoS."""
         if self.source == "wos":
             use_cols = ["I2", "LCS", "TC"]
-        else:
-            raise ValueError("Invalid source type")
         return self.generate_df_factory(use_cols, "I2", "; ")
 
-    def generate_co_df(self) -> pd.DataFrame:
+    def generate_country_df(self) -> pd.DataFrame:
         """Return country DataFrame. Only support WoS."""
         if self.source == "wos":
             use_cols = ["CO", "LCS", "TC"]
-        else:
-            raise ValueError("Invalid source type")
         return self.generate_df_factory(use_cols, "CO", "; ")
 
     def generate_journal_df(self) -> pd.DataFrame:
         """Return journal DataFrame."""
-        if self.source in ["wos", "scopus"]:
-            use_cols = ["SO", "LCS", "TC"]
-        elif self.source == "cssci":
-            use_cols = ["SO", "LCS"]
-        else:
-            raise ValueError("Invalid source type")
+        use_cols = ["SO", "LCS", "TC"]
+        if self.source == "cssci":
+            use_cols.remove("TC")
         return self.generate_df_factory(use_cols, "SO")
 
     def generate_year_df(self) -> pd.DataFrame:
-        """Return publication year DataFrame. Sort by `PY` ascending."""
+        """Return publication year DataFrame."""
         use_cols = ["PY"]
         return self.generate_df_factory(use_cols, "PY").sort_values(by="PY")
 
     def generate_document_type_df(self) -> pd.DataFrame:
         """Return document type DataFrame. Not support CSSCI."""
-        assert self.source != "cssci", "CSSCI doesn't have <document type> info"
         use_cols = ["DT"]
         return self.generate_df_factory(use_cols, "DT")
 
     def write2excel(self, save_path: Path):
         """Write all dataframes to an excel file. Each dataframe is a sheet.
 
         Args:
@@ -233,15 +193,19 @@
         with pd.ExcelWriter(save_path) as writer:
             self.generate_record_df().to_excel(writer, sheet_name="Records", index=False)
             self.generate_author_df().to_excel(writer, sheet_name="Authors")
             self.generate_journal_df().to_excel(writer, sheet_name="Journals")
             self.generate_keyword_df().to_excel(writer, sheet_name="Keywords")
             self.generate_year_df().to_excel(writer, sheet_name="Yearly output")
 
-            if self.source in ["wos", "scopus"]:
+            if self.source == "wos":
                 self.generate_document_type_df().to_excel(writer, sheet_name="Document Type")
-            if self.source in ["wos", "cssci"]:
                 self.generate_institution_df().to_excel(writer, sheet_name="Institution")
-            if self.source in ["wos"]:
-                self.generate_i2_df().to_excel(writer, sheet_name="Institution with Subdivision")
-                self.generate_co_df().to_excel(writer, sheet_name="Country")
+                self.generate_sub_institution_df().to_excel(writer, sheet_name="Institution with Subdivision")
+                self.generate_country_df().to_excel(writer, sheet_name="Country")
                 self.generate_corresponding_author_df().to_excel(writer, sheet_name="Corresponding Authors")
+
+            elif self.source == "scopus":
+                self.generate_document_type_df().to_excel(writer, sheet_name="Document Type")
+
+            elif self.source == "cssci":
+                self.generate_institution_df().to_excel(writer, sheet_name="Institution")
```

### Comparing `histcite-python-1.1.0/histcite/read_file.py` & `histcite_python-2.0.0/histcite/read_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,119 +4,112 @@
 - Web of Science: savedrecs.txt
 - CSSCI: LY_.txt
 - Scopus: scopus.csv
 """
 
 import re
 from pathlib import Path
-from typing import Callable, Literal, Optional
+from typing import Literal, Optional
 
 import pandas as pd
 
 
 def read_csv_file(file_path: Path, use_cols: list[str], sep: str = ",") -> pd.DataFrame:
-    """Read csv file using `pyarrow` backend."""
     try:
         df = pd.read_csv(
             file_path,
             sep=sep,
             header=0,
             on_bad_lines="skip",
             usecols=use_cols,
-            dtype_backend="pyarrow",
+            # dtype_backend="pyarrow",
         )
         return df
     except ValueError:
         raise ValueError(f"File {file_path.name} is not a valid csv file")
 
 
 class ReadWosFile:
     @staticmethod
-    def extract_first_author(au_field: pd.Series) -> pd.Series:
-        return au_field.str.split(pat=";", n=1, expand=True)[0].str.replace(",", "")
-
-    @staticmethod
-    def extract_corresponding_authors(entry: Optional[str]) -> Optional[str]:
-        """Extract corresponding authors from RP value."""
-        pattern = r"(?:^|\.; )(.+?)\s*\(corresponding author\)"
-        if entry is not None:
+    def extract_corresponding_author(entry: Optional[str]) -> Optional[str]:
+        """Extract corresponding author from RP value."""
+        if isinstance(entry, str):
             cau_list = []
+            pattern = r"(?:^|\.; )(.+?)\s*\(corresponding author\)"
             for cau in re.findall(pattern, entry):
                 if "; " in cau:
                     cau_list.extend(cau.split("; "))
                 else:
                     cau_list.append(cau)
-        return "; ".join(set(cau_list))
+            return "; ".join(set(cau_list))
 
     @staticmethod
-    def extract_co_i2(entry: Optional[str]) -> tuple[Optional[str], Optional[str]]:
-        """Extract country and institution with subdivision from C1 or RP value"""
-        co_value = None
-        i2_value = None
-        if entry is not None:
-            if "corresponding author" in entry:
-                pattern = r"\(corresponding author\), (.*?)\.(?=;|$)"
-            else:
-                pattern = r"\] (.*?)(?=; \[|$)"
-            addr_list = re.findall(pattern, entry)
+    def extract_country(entry: Optional[str]) -> Optional[str]:
+        """Extract country info from C1 value."""
+        if isinstance(entry, str):
+            addr_list = re.findall(r"\] (.*?)(?=;|$)", entry)
+            if len(addr_list) > 0:
+                country_list = [addr.rsplit(", ", 1)[1] for addr in addr_list]
+                country_list = ["USA" if country.endswith(" USA") else country for country in country_list]
+                return "; ".join(set(country_list))
+
+    @staticmethod
+    def extract_sub_institution(entry: Optional[str]) -> Optional[str]:
+        """Extract sub institution from C1 value"""
+        if isinstance(entry, str):
+            addr_list = re.findall(r"\] (.*?)(?=;|$)", entry)
             if len(addr_list) > 0:
-                co_set = set()
-                i2_set = set()
+                institution_list = []
                 for addr in addr_list:
-                    parts = addr.split(", ")
-                    i2 = ", ".join(parts[:2]) if len(parts) > 3 else parts[0]
-                    co = parts[-1]
-                    if co[-4:] == " USA":
-                        co = "USA"
-                    co_set.add(co)
-                    i2_set.add(i2)
-                co_value = "; ".join(co_set)
-                i2_value = "; ".join(i2_set)
-        return co_value, i2_value
+                    if addr.count(", ") >= 3:
+                        institution = ", ".join(addr.split(", ", 2)[:2])
+                    else:
+                        institution = addr.split(", ", 1)[0]
+                    institution_list.append(institution)
+                return "; ".join(set(institution_list))
 
     @staticmethod
-    def read_wos_file(file_path: Path, addr_field: Literal["C1", "RP"]) -> pd.DataFrame:
+    def read_wos_file(file_path: Path) -> pd.DataFrame:
         """Read Web of Science file and return dataframe.
 
         Args:
             file_path: Path of a Web of Science file. File name is similar to `savedrecs.txt`.
-            addr_field: Which address field to use to extract institution with subdivision and country info.
         """
         use_cols = [
             "AU",
             "TI",
             "SO",
             "DT",
             "CR",
             "DE",
             "C3",
             "NR",
             "TC",
-            "J9",
             "PY",
             "VL",
             "BP",
             "DI",
             "UT",
             "C1",
             "RP",
         ]
         df = read_csv_file(file_path, use_cols, "\t")
-        df.insert(1, "FAU", ReadWosFile.extract_first_author(df["AU"]))
-        df.insert(2, "CAU", df["RP"].apply(ReadWosFile.extract_corresponding_authors))
-        df[["CO", "I2"]] = df[addr_field].apply(ReadWosFile.extract_co_i2).apply(pd.Series)
+        df.insert(1, "FAU", df["AU"].str.split(pat=";", n=1).str[0].str.replace(",", ""))
+        df.insert(2, "CAU", df["RP"].apply(ReadWosFile.extract_corresponding_author))
+        df["CO"] = df["C1"].apply(ReadWosFile.extract_country)
+        df["I2"] = df["C1"].apply(ReadWosFile.extract_sub_institution)
         df["source file"] = file_path.name
         return df
 
 
 class ReadCssciFile:
     @staticmethod
-    def extract_org(org_cell: str) -> str:
-        org_set = set(re.findall(r"](.*?)(?:/|$)", org_cell))
-        return "; ".join([i.replace(".", "") for i in org_set])
+    def extract_org(entry: str) -> str:
+        org_list = re.findall(r"](.*?)(?:/|$)", entry)
+        return "; ".join(set(org_list))
 
     @staticmethod
     def read_cssci_file(file_path: Path) -> pd.DataFrame:
         """Read CSSCI file and return dataframe. Use `WOS` fields to replace original fields.
 
         Args:
             file_path: Path of a CSSCI file. File name is similar to `LY_.txt`.
@@ -150,23 +143,23 @@
         column_mapping = {
             "来源篇名": "TI",
             "来源作者": "AU",
             "基    金": "FU",
             "期    刊": "SO",
             "机构名称": "C3",
             "第一作者": "FAU",
-            "年代卷期": "PY&VL&BP&EP",
+            "年代卷期": "MIX",
             "关 键 词": "DE",
             "参考文献": "CR",
         }
         df.rename(columns=column_mapping, inplace=True)
 
         df["AU"] = df["AU"].str.replace("/", "; ")
         df["DE"] = df["DE"].str.replace("/", "; ")
-        df["PY"] = df["PY&VL&BP&EP"].str.extract(r"^(\d{4}),", expand=False)
+        df["PY"] = df["MIX"].str.extract(r"^(\d{4}),")
         df["C3"] = df["C3"].apply(ReadCssciFile.extract_org)
         df["CR"] = df["CR"].str.replace("\n", "; ")
         df["NR"] = df["CR"].str.count("; ") + 1
         df.insert(2, "FAU", df.pop("FAU"))
         df["source file"] = file_path.name
         return df
 
@@ -177,15 +170,14 @@
         """Read Scopus file and return dataframe. Use `WOS` fields to replace original fields.
 
         Args:
             file_path: Path of a Scopus file. File name is similar to `scopus.csv`.
         """
         use_cols = [
             "Authors",
-            "Author full names",
             "Title",
             "Year",
             "Source title",
             "Volume",
             "Issue",
             "Page start",
             "Page end",
@@ -213,76 +205,61 @@
             "Author Keywords": "DE",
             "References": "CR",
             "Document Type": "DT",
         }
         df.rename(columns=column_mapping, inplace=True)
 
         df["NR"] = df["CR"].str.count("; ")
-        df.insert(1, "FAU", df["AU"].str.split(pat=";", n=1, expand=True)[0])
+        df.insert(1, "FAU", df["AU"].str.split(pat=";", n=1).str[0])
         df["source file"] = file_path.name
         return df
 
 
 class ReadFile:
     """Read files in the folder path and return a concated dataframe."""
 
-    def __init__(
-        self, folder_path: Path, source: Literal["wos", "cssci", "scopus"], addr_field: Literal["C1", "RP"] = "C1"
-    ):
+    def __init__(self, folder_path: Path, source: Literal["wos", "cssci", "scopus"]):
         """
         Args:
             folder_path: The folder path of raw files.
             source: Data source. `wos`, `cssci` or `scopus`.
-            addr_field: Address field, only for wos source. `C1` or `RP`.
         """
         self.folder_path: Path = folder_path
         self.source: Literal["wos", "cssci", "scopus"] = source
-        self.addr_field = addr_field
         try:
             self.file_path_list: list[Path] = self.obtain_file_path_list()
         except FileNotFoundError:
             raise FileNotFoundError(f"{folder_path} 文件夹不存在")
 
     def obtain_file_path_list(self) -> list[Path]:
         if self.source == "wos":
-            file_name_list = [i for i in self.folder_path.iterdir() if i.name.startswith("savedrecs")]
+            file_name_list = [i for i in self.folder_path.iterdir() if i.name.startswith("savedrecs") and i.suffix == ".txt"]
         elif self.source == "cssci":
-            file_name_list = [i for i in self.folder_path.iterdir() if i.name.startswith("LY_")]
+            file_name_list = [i for i in self.folder_path.iterdir() if i.name.startswith("LY_") and i.suffix == ".txt"]
         elif self.source == "scopus":
-            file_name_list = [i for i in self.folder_path.iterdir() if i.name.startswith("scopus")]
+            file_name_list = [i for i in self.folder_path.iterdir() if i.name.startswith("scopus") and i.suffix == ".csv"]
         else:
             raise ValueError("Invalid data source")
         file_name_list.sort()
         return file_name_list
 
-    def concat_df(self) -> pd.DataFrame:
+    def read_file(self, file_path: Path):
+        if self.source == "wos":
+            return ReadWosFile.read_wos_file(file_path)
+        elif self.source == "scopus":
+            return ReadScopusFile.read_scopus_file(file_path)
+        elif self.source == "cssci":
+            return ReadCssciFile.read_cssci_file(file_path)
+
+    def concat_files(self):
         file_count = len(self.file_path_list)
         if file_count > 1:
-            if self.source == "wos":
-                return pd.concat(
-                    [ReadWosFile.read_wos_file(file_path, self.addr_field) for file_path in self.file_path_list],
-                    ignore_index=True,
-                )
-            elif self.source == "cssci":
-                return pd.concat(
-                    [ReadCssciFile.read_cssci_file(file_path) for file_path in self.file_path_list],
-                    ignore_index=True,
-                )
-            elif self.source == "scopus":
-                return pd.concat(
-                    [ReadScopusFile.read_scopus_file(file_path) for file_path in self.file_path_list],
-                    ignore_index=True,
-                )
+            return pd.concat([self.read_file(file_path) for file_path in self.file_path_list], ignore_index=True)
         elif file_count == 1:
-            if self.source == "wos":
-                return ReadWosFile.read_wos_file(self.file_path_list[0], self.addr_field)
-            elif self.source == "cssci":
-                return ReadCssciFile.read_cssci_file(self.file_path_list[0])
-            elif self.source == "scopus":
-                return ReadScopusFile.read_scopus_file(self.file_path_list[0])
+            return self.read_file(self.file_path_list[0])
         else:
             raise FileNotFoundError("No valid file in the folder")
 
     @staticmethod
     def drop_duplicate_rows(docs_df: pd.DataFrame, check_cols: list[str]) -> pd.DataFrame:
         original_num = docs_df.shape[0]
         try:
@@ -296,16 +273,17 @@
             return docs_df
 
     def read_all(self) -> pd.DataFrame:
         """Concat multi dataframe and drop duplicate rows."""
         if self.source == "wos":
             check_cols = ["UT"]
         elif self.source == "cssci":
-            check_cols = ["TI", "FAU"]
+            check_cols = ["FAU", "TI"]
         elif self.source == "scopus":
             check_cols = ["EID"]
 
-        docs_df = self.concat_df()
+        docs_df = self.concat_files()
+        assert docs_df is not None, "Something wrong happened when reading files."
         docs_df = self.drop_duplicate_rows(docs_df, check_cols)
-        docs_df.insert(0, "doc_id", docs_df.index)
+        docs_df.insert(0, "node", docs_df.index)
         docs_df = docs_df.convert_dtypes(dtype_backend="pyarrow")
         return docs_df
```

### Comparing `histcite-python-1.1.0/histcite_python.egg-info/PKG-INFO` & `histcite_python-2.0.0/histcite_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 1.1.0
+Version: 2.0.0
 Summary: A Python interface for histcite
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/doublessay/histcite-python
 Keywords: histcite,citation network,web of science,scopus,cssci
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -20,58 +20,58 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=2.0
 Requires-Dist: pyarrow
 Requires-Dist: openpyxl
+Requires-Dist: refparse
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
-# HistCite工具的Python实现
+# HistCite 工具的 Python 实现
 
 [![PyPI](https://img.shields.io/pypi/v/histcite-python)](https://pypi.org/project/histcite-python)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/histcite-python.svg)](https://pypi.org/project/histcite-python)
 [![Codecov](https://codecov.io/gh/doublessay/histcite-python/graph/badge.svg?token=99V9E2CI1H)](https://codecov.io/gh/doublessay/histcite-python)
 [![License](https://img.shields.io/pypi/l/histcite-python.svg)](https://github.com/doublessay/histcite-python/blob/main/LICENSE)
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内使用较多的为中科大某同学 (知乎昵称[Tsing](https://www.zhihu.com/people/wq123)) 在源程序基础上修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅适用于 `Windows` 平台，存在较大限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具实现了 `HistCite` 的核心功能，可以跨平台使用，同时拓展了对 [其他数据源](#数据准备) 的支持。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内使用较多的为中科大某同学 (知乎昵称 [Tsing](https://www.zhihu.com/people/wq123)) 在源程序基础上修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅适用于 `Windows` 平台，存在较大限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具实现了 `HistCite` 的核心功能，可以跨平台使用，同时拓展了对 [其他数据源](#数据准备) 的支持。
 
 核心功能：
 - 生成引文网络图；
 - 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
-- 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 工具对比：
 |对比项|histcite-python|histcite pro|
 |:----|:----|:----|
 |是否开源|是|否|
 |是否跨平台|是|否，仅限 Windows|
 |是否支持其他数据源|是|否，仅限 Web of Science|
-|是否提供前端界面|否|是|
+|是否提供前端界面|否|是，可交互|
 |引文网络图|矢量图，比较清晰|位图，比较模糊|
 
 ## 快速开始
 ```console
-pip install histcite-python
+$ pip install histcite-python
 ```
 
 ## 数据准备
 |数据来源|下载说明|原始文件名|
 |:----|:----|:----|
 |Web of Science|`核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custom selection/自定义选择项`，全选字段。|`savedrecs*.txt`|
 |CSSCI|从 `CSSCI数据库` 正常导出即可。|`LY_*.txt`|
-|Scopus|格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。|`scopus*.csv`|
+|Scopus|网站语言切换到英文，格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。|`scopus*.csv`|
 
 > [!WARNING]
-> 文件下载后不要重命名(会根据文件名识别有效的题录数据文件)，把下载的所有文件放在一个单独的文件夹内。
+> 文件下载后不要重命名(会根据文件名识别有效的数据文件)，把下载的所有文件放在一个单独的文件夹内。
 
 ## 使用方法
 1. 使用命令行工具
 ```console
 $ histcite -h
 usage: histcite [-h] (--top TOP | --threshold THRESHOLD | --node NODE) [--disable_timeline] folder_path {wos,cssci,scopus}
 
@@ -85,80 +85,74 @@
   -h, --help            show this help message and exit
   --top                 Top N nodes with the highest LCS.
   --threshold           Nodes with LCS greater than threshold.
   --disable_timeline    Whether to disable timeline.
 ```
 
 ```console
-$ histcite /Users/.../Downloads/dataset wos --top 100 --disable_timeline
+$ histcite /Users/.../Downloads/dataset wos --top 50 --disable_timeline
 ```
 
 > [!NOTE]
 > 生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含
-> - 描述统计表 descriptive_statistics.xlsx
 > - 引文网络图节点信息表 graph_node_info.xlsx
 > - 引文网络图的数据文件 graph.dot
->     - 借助 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+>     - 借助 [Graphviz 在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz](https://graphviz.org/) 生成引文网络图。
 
 引文网络图示例：
 
 ![](https://raw.githubusercontent.com/doublessay/histcite-python/main/examples/graph.svg)
 
-对应的节点信息如下(以CSSCI数据源为例，不同文献数据库的节点信息字段存在差异)：
+对应的节点信息如下(以 CSSCI 数据源为例)：
 | |AU|TI|PY|SO|LCS|
 |:----|:----|:----|:----|:----|:----|
 |55|张坤; 查先进|我国智慧图书馆的发展沿革及构建策略研究|2021|国家图书馆学刊|6|
 |60|石婷婷; 徐建华; 张雨浓|数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计|2021|情报理论与实践|7|
 |63|卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷|智慧图书馆建设标准探析|2021|中国图书馆学报|9|
 |81|程焕文; 钟远薪|智慧图书馆的三维解析|2021|图书馆论坛|10|
 |86|段美珍; 初景利; 张冬荣; 解贺嘉|智慧图书馆的内涵特点及其认知模型研究|2021|图书情报工作|7|
 |...| | | | | |
 
-2. 使用 Jupyter，比命令行更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+2. 使用 Jupyter Notebook，可以自定义更多参数，导出描述性统计数据，请查看 [demo.ipynb](demo.ipynb)
 
 ## 字段说明
 |Field Name|Description|
 |:----|:----|
 |`GCS`|Global Citation Score, 表示一篇文献在文献数据库中的总被引次数|
 |`LCS`|Local Citation Score, 表示一篇文献在本地文献集中的被引次数|
 |`GCR`|Global Cited References, 表示一篇文献的参考文献数量|
 |`LCR`|Local Cited References, 表示一篇文献的参考文献在本地文献集中的数量|
 |`T*` |Total score, e.g. TLCS = Total Local Citation Scores.|
 |`Recs`|Count of Records|
 |`FAU`|First Author|
 |`CAU`|Corresponding Authors|
 |`AU`|Authors|
-|`EM`|Email Address|
 |`CO`|Country of Authors|
 |`C1`|Addresses|
 |`C3`|Author Affiliations|
 |`RP`|Reprint Address|
 |`I2`|Institution with Subdivision|
 |`TI`|Article Title|
 |`SO`|Source Title|
 |`DT`|Document Type|
-|`FU`|Funding Orgs|
 |`DE`|Author Keywords|
 |`CR`|Cited References|
 |`NR`|Cited Reference Count|
 |`TC`|Times Cited Count|
-|`J9`|Journal Abbreviation|
 |`PY`|Publication Year|
 |`VL`|Volume|
 |`IS`|Issue|
 |`BP`|Start Page|
 |`EP`|End Page|
 |`DI`|DOI|
 |...|[Please refer to Web of Science fields.](https://webofscience.help.clarivate.com/en-us/Content/export-records.htm)|
 
 ## FAQ
 1. 为什么生成的引文网络图时间线会错乱？
-- Graphviz 会自动调整节点位置，节点数量较少时容易出现这一问题。可以通过设置参数来关闭时间线。
+- 节点位置由 Graphviz 自动调整，节点数量较少时容易出现这一问题。可以通过设置参数隐藏时间线。
 
-2. 想要分析其他来源的文献元数据？
-- 该数据源能够导出文献的参考文献或引文数据。如果满足这一条件的话，欢迎提交 [Feature Request](https://github.com/doublessay/histcite-python/issues)，我们会尽快支持。
-
-3. 是否存在其他类似的工具？
+2. 是否存在其他类似的工具？
 - [CiteSpace](https://citespace.podia.com/)
 - [CitNetExplorer](https://www.citnetexplorer.nl/)
+- [VOSviewer](https://www.vosviewer.com/)
 - [Connected Papers](https://www.connectedpapers.com/)
 - [Litmaps](https://app.litmaps.com/)
```

### Comparing `histcite-python-1.1.0/pyproject.toml` & `histcite_python-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     ]
 dynamic = ["version"]
 
 dependencies = [
     "pandas>=2.0",
     "pyarrow",
     "openpyxl",
+    "refparse",
     ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "coverage",
     "mypy",
@@ -59,8 +60,8 @@
 [tool.setuptools.dynamic]
 version = {attr = "histcite.__version__"}
 
 [tool.coverage.run]
 source = ["histcite"]
 
 [tool.black]
-line-length = 120
+line-length = 140
```

