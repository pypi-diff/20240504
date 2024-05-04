# Comparing `tmp/pyqueen-1.0.8.tar.gz` & `tmp/pyqueen-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqueen-1.0.8.tar", last modified: Tue Nov 14 06:48:52 2023, max compression
+gzip compressed data, was "pyqueen-1.0.9.tar", last modified: Wed Nov 22 07:55:41 2023, max compression
```

## Comparing `pyqueen-1.0.8.tar` & `pyqueen-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:52.688629 pyqueen-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-14 06:48:36.000000 pyqueen-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2023-11-14 06:48:52.688629 pyqueen-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2023-11-14 06:48:36.000000 pyqueen-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:52.684629 pyqueen-1.0.8/pyqueen/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:52.688629 pyqueen-1.0.8/pyqueen/etl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9299 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/etl/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/etl/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/etl/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/etl/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/etl/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:52.688629 pyqueen-1.0.8/pyqueen/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/service/pydingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/service/pyemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/service/pywechat.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/service/showdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:52.688629 pyqueen-1.0.8/pyqueen/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/utility/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9595 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/utility/time_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-11-14 06:48:36.000000 pyqueen-1.0.8/pyqueen/utility/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 06:48:52.688629 pyqueen-1.0.8/pyqueen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2023-11-14 06:48:52.000000 pyqueen-1.0.8/pyqueen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-11-14 06:48:52.000000 pyqueen-1.0.8/pyqueen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 06:48:52.000000 pyqueen-1.0.8/pyqueen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-14 06:48:52.000000 pyqueen-1.0.8/pyqueen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-14 06:48:52.000000 pyqueen-1.0.8/pyqueen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-14 06:48:52.000000 pyqueen-1.0.8/pyqueen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 06:48:52.688629 pyqueen-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-11-14 06:48:36.000000 pyqueen-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.199183 pyqueen-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-22 07:55:31.000000 pyqueen-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2023-11-22 07:55:41.199183 pyqueen-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9565 2023-11-22 07:55:31.000000 pyqueen-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.191183 pyqueen-1.0.9/pyqueen/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.195183 pyqueen-1.0.9/pyqueen/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/analysis/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.195183 pyqueen-1.0.9/pyqueen/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/io/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.195183 pyqueen-1.0.9/pyqueen/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/pydingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/pyemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/pywechat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/service/showdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.199183 pyqueen-1.0.9/pyqueen/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9595 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/time_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-11-22 07:55:31.000000 pyqueen-1.0.9/pyqueen/utility/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 07:55:41.199183 pyqueen-1.0.9/pyqueen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-22 07:55:41.000000 pyqueen-1.0.9/pyqueen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-22 07:55:41.199183 pyqueen-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2023-11-22 07:55:31.000000 pyqueen-1.0.9/setup.py
```

### Comparing `pyqueen-1.0.8/LICENSE` & `pyqueen-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/PKG-INFO` & `pyqueen-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,45 @@
-Metadata-Version: 2.1
-Name: pyqueen
-Version: 1.0.8
-Summary: Rule your Data
-Home-page: https://github.com/ts7ming/pyqueen.git
-Author: ts7ming
-Author-email: qiming.ma@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: requests
-Requires-Dist: SQLAlchemy==1.4.49
-Requires-Dist: xlrd==1.2.0
-Requires-Dist: XlsxWriter
-
 # PyQueen
+
 ![](logo.jpg)
 
 ![github license](https://img.shields.io/github/license/ts7ming/pyqueen)
 [![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)
 ![Language](https://img.shields.io/badge/language-Python-brightgreen)
 [![Documentation Status](https://readthedocs.org/projects/pyqueen/badge/?version=latest)](https://pyqueen.readthedocs.io/zh-cn/latest/?badge=latest)
 ![GitHub Repo stars](https://img.shields.io/github/stars/ts7ming/pyqueen)
+[![PyPI downloads](https://img.shields.io/pypi/dm/pyqueen.svg)](https://pypistats.org/packages/pyqueen)
 
-PyQueen 是一个简单的数据处理工具箱. 配合 Pandas 使用可以完成简单的ETL作业
+PyQueen 是一个数据处理工具箱. 配合 Pandas 使用可以完成简单的ETL作业
 
 ## Install
+
 ```bash
 pip install pyqueen
 ```
 
 ## Doc
+
 - [readthedocs](https://pyqueen.readthedocs.io/zh-cn/latest/)
 - 示例: example/*
 
 #### 读写数据库
+
 - dbtype: 可选 mysql,mssql,oracle,clickhouse,sqlite
 - 每次操作数据库都会销毁连接, 无需关注连接池情况
-  - 如需主动控制连接 使用: `ds.keep_conn()` 和 `ds.close_conn()`
+    - 如需主动控制连接 使用: `ds.keep_conn()` 和 `ds.close_conn()`
 - 如需切换 db_name 使用: `ds.set_db(db_name)`
 - 设置字符集 使用: `ds.set_charset(charset)`. 默认: `utf8mb4`
 - 设置 chunksize 使用 `ds.set_chunksize(1000)`. 默认: `10000`
 - 数据库连接支持
-  - mysql: `pip install pymysql`
-  - mssql: `pip install pymssql` 
-    - 可选 `pip install pyodbc` 需指定 `ds.set_package('pyodbc')`
-  - oracle: `pip install cx_oracle`
-  - clickhouse: `pip install clickhouse-driver`
+    - mysql: `pip install pymysql`
+    - mssql: `pip install pymssql`
+        - 可选 `pip install pyodbc` 需指定 `ds.set_package('pyodbc')`
+    - oracle: `pip install cx_oracle`
+    - clickhouse: `pip install clickhouse-driver`
 
 ```python
 from pyqueen import DataSource
 
 ds = DataSource(host='', username='', password='', port='', db_name='', db_type='')
 
 # 根据sql查询, 返回 pd.DataFrame 对象
@@ -72,53 +58,64 @@
 # pd.DataFrame 转图片
 ### 可以指定文件路径: file_path. 默认生成临时文件
 ### 可以用列表为每一列指定宽度 col_width
 ### 指定字体大小 font_size
 path = ds.to_image(df, file_path=None, col_width=None, font_size=None)
 ```
 
+#### 常用模型
+
+```python
+from pyqueen import Model
+
+data = df['待预测列']  # 也可以是 list形式的数据
+### forecast_step: 预测节点数
+### p,d,q: 自定义arima模型参数. 为空时自动使用最优模型
+forecast_result = Model.arima(data, forecast_step=10, p=None, d=None, q=None)
+```
 #### ETL辅助功能
+
 ```python
 # 使用SQL语法查询 pd.DataFrame 数据 (功能依赖duckdb包); 可以部分代替 pandas接口 
 ### 等价python
 df_fact = pd.merge(df_fact, df_dim1, on='d1', how='inner')
 df_fact = pd.merge(df_fact, df_dim1, on='d2', how='inner')
-df_summary = df_fact.groupby(['d1_name','d2_name']).agg({'value':np.sum}).reset_index().rename('value':'sum_value')
+df_summary = df_fact.groupby(['d1_name', 'd2_name']).agg({'value': np.sum}).reset_index().rename('value':'sum_value')
 
 ### 可以用sql实现
 from pyqueen import DataSource
+
 ds = DataSource()
 data = {'table1': df_fact, 'table2': df_dim1, 'table3': df_dim2}
 sql = '''
   select b.d1_name,c.d2_name,sum(a.value) as sum_value
   from table1 a 
   inner join table2 b on a.d1 = b.d1
   inner join table3 c on a.d2 = c.d2
   group by b.d1_name,c.d2_name
 '''
 df_summary = ds.pdsql(sql=sql, data=data)
 
-
 # 导入测试数据
 ### 会将excel文件里的每一个sheet映射成一张表, 将这个 ds 后续的sql查询都转移到这个由excel文件生成的新数据库
 ### 用于测试确认复杂计算逻辑, 相当于用excel文件代替测试数据库
 ds.import_test_data(excel_path='')
 ```
 
-
 #### 下载FTP文件
 
 ```python
 from pyqueen import DataSource
 
 ds = DataSource(host='', username='', password='', port='', db_type='ftp')
 ds.download_ftp(local_dir='保存目录', remote_dir='远程目录')
 ```
 
 #### 写入Excel文件
+
 - 将 pd.DataFrame对象 写入Excel文件
 - file_path 文件路径 (须以 .xlsx 结尾)
 - sheet_list 待写入数据, 二维列表, 每个 pd.DataFrame对象 对应一个 sheet
 - fillna='' 空值填充
 - fmt=None 字段格式,可以按字段名指定
 - font='微软雅黑' 字体
 - font_color='black' 字体颜色
@@ -141,39 +138,40 @@
     'col4': '0.00%',
     'col5': 'YYYY-MM-DD'
 }
 ds.to_excel(file_path='xxx.xlsx', sheet_list=sheet_list, fmt=fmt)
 ```
 
 #### 时间处理工具
+
 ```python
 from pyqueen import TimeKit
 
 # 按当前时间
 tk = TimeKit()
 # 指定日期, 时间
 tk = TimeKit(theday=20200101, thetime=120000)
 
 # 常用属性
-tk.today    # 当前日期或初始化指定日期
-tk.now    # 当前时间或初始化指定时间
-tk.hour    # 当前小时
-tk.minute    # 当前分钟
-tk.second    # 当前秒
-tk.nday_of_week    # 1-7对应周一到周日
-tk.week_start    # 本周一日期
-tk.lw_start    # 上周开始日期
-tk.lw_end    # 上周结束日期
-tk.lw2_start    # 上上周开始日期
-tk.lw2_end    # 上上周结束日期
-tk.month_start    # 本月初
-tk.lm_start    # 上月初
-tk.lm_end    # 上月末
-tk.lm2_start    # 上上月初
-tk.lm2_end    # 上上月末
+tk.today  # 当前日期或初始化指定日期
+tk.now  # 当前时间或初始化指定时间
+tk.hour  # 当前小时
+tk.minute  # 当前分钟
+tk.second  # 当前秒
+tk.nday_of_week  # 1-7对应周一到周日
+tk.week_start  # 本周一日期
+tk.lw_start  # 上周开始日期
+tk.lw_end  # 上周结束日期
+tk.lw2_start  # 上上周开始日期
+tk.lw2_end  # 上上周结束日期
+tk.month_start  # 本月初
+tk.lm_start  # 上月初
+tk.lm_end  # 上月末
+tk.lm2_start  # 上上月初
+tk.lm2_end  # 上上月末
 
 # 时间加减
 # flag: 加减单位: years,months,days,hours,minutes,seconds
 # value: 加减值
 # thetime之前 value 写负值
 # thetime之后 value 写正值
 new_day = tk.time_delta('20230101', 'days', -30)
@@ -189,14 +187,15 @@
 # 查询任意日期是星期几
 n = tk.get_nday_of_week(20200101)
 # 数值型日期转字符串
 date_str = tk.int2str(20200101, sep='-')
 ```
 
 #### ETL日志
+
 - 记录所有 `DataSource` 类函数的调用过程和相应参数
 - 如需启用日志, 添加: `ds.set_logger(logger)`
 - 其中 `logger` 为日志处理函数, 默认为: `print`
 - 自定义 `logger` 参考 `example/etl_with_log.py`
 - `etl_log` 所有 **key**
     - py_path: 调用脚本路径
     - func_name: 调用函数名
@@ -209,14 +208,15 @@
     - host: (如有) 服务器地址
     - db_type: (如有) 数据库类型
     - port: (如有) 端口
     - db_name: (如有) 数据库名
     - table_name: (如有) 表名
 
 #### 发送信息
+
 - 邮件
 - 钉钉
 - 企业微信
 
 ```python
 from pyqueen import Email
 
@@ -257,14 +257,15 @@
 # content不为None时,发送文本
 # mentioned_list: userid的列表，提醒群中的指定成员(@某个成员)，@all表示提醒所有人
 # mentioned_mobile_list: 手机号列表，提醒手机号对应的群成员(@某个成员)，@all表示提醒所有人
 wechat.send(content=None, mentioned_list=None, mentioned_mobile_list=None)
 ```
 
 #### 小工具
+
 ```python
 from pyqueen import Utils
 
 # 压缩/解压缩
 Utils.zip(from_path='', to_path='')
 Utils.unzip(from_path='', to_path='')
 # 删除文件
@@ -283,18 +284,19 @@
 ### args_list: 每个子任务的参数
 ### max_process = 1: 最大进程数, 默认为 1
 ### 以list返回每个子进程执行结果, 和 args_list 顺序一致
 result = Utils.mult_run(func, args_list=[], max_process=1)
 ```
 
 #### 命令行
+
 ```commandline
 用法: pyqueen command args1,args2,...
 ---
 command: 
     #1  sql2table [file_path] 从sql解析用到的表(通过正则解析, 有误差) (不带参数时读取剪切板)
     
-    #2  getcode file_path: 检测文件编码
+    #2  detcode file_path: 检测文件编码
     
-    #3 md5 基于剪切板文本生成md5
+    #3  md5 基于剪切板文本生成md5
 ```
```

### Comparing `pyqueen-1.0.8/README.md` & `pyqueen-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,64 @@
+Metadata-Version: 2.1
+Name: pyqueen
+Version: 1.0.9
+Summary: Rule your Data
+Home-page: https://github.com/ts7ming/pyqueen.git
+Author: ts7ming
+Author-email: qiming.ma@outlook.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: SQLAlchemy==1.4.49
+Requires-Dist: xlrd==1.2.0
+Requires-Dist: XlsxWriter
+
 # PyQueen
+
 ![](logo.jpg)
 
 ![github license](https://img.shields.io/github/license/ts7ming/pyqueen)
 [![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)
 ![Language](https://img.shields.io/badge/language-Python-brightgreen)
 [![Documentation Status](https://readthedocs.org/projects/pyqueen/badge/?version=latest)](https://pyqueen.readthedocs.io/zh-cn/latest/?badge=latest)
 ![GitHub Repo stars](https://img.shields.io/github/stars/ts7ming/pyqueen)
+[![PyPI downloads](https://img.shields.io/pypi/dm/pyqueen.svg)](https://pypistats.org/packages/pyqueen)
 
-PyQueen 是一个简单的数据处理工具箱. 配合 Pandas 使用可以完成简单的ETL作业
+PyQueen 是一个数据处理工具箱. 配合 Pandas 使用可以完成简单的ETL作业
 
 ## Install
+
 ```bash
 pip install pyqueen
 ```
 
 ## Doc
+
 - [readthedocs](https://pyqueen.readthedocs.io/zh-cn/latest/)
 - 示例: example/*
 
 #### 读写数据库
+
 - dbtype: 可选 mysql,mssql,oracle,clickhouse,sqlite
 - 每次操作数据库都会销毁连接, 无需关注连接池情况
-  - 如需主动控制连接 使用: `ds.keep_conn()` 和 `ds.close_conn()`
+    - 如需主动控制连接 使用: `ds.keep_conn()` 和 `ds.close_conn()`
 - 如需切换 db_name 使用: `ds.set_db(db_name)`
 - 设置字符集 使用: `ds.set_charset(charset)`. 默认: `utf8mb4`
 - 设置 chunksize 使用 `ds.set_chunksize(1000)`. 默认: `10000`
 - 数据库连接支持
-  - mysql: `pip install pymysql`
-  - mssql: `pip install pymssql` 
-    - 可选 `pip install pyodbc` 需指定 `ds.set_package('pyodbc')`
-  - oracle: `pip install cx_oracle`
-  - clickhouse: `pip install clickhouse-driver`
+    - mysql: `pip install pymysql`
+    - mssql: `pip install pymssql`
+        - 可选 `pip install pyodbc` 需指定 `ds.set_package('pyodbc')`
+    - oracle: `pip install cx_oracle`
+    - clickhouse: `pip install clickhouse-driver`
 
 ```python
 from pyqueen import DataSource
 
 ds = DataSource(host='', username='', password='', port='', db_name='', db_type='')
 
 # 根据sql查询, 返回 pd.DataFrame 对象
@@ -53,53 +77,64 @@
 # pd.DataFrame 转图片
 ### 可以指定文件路径: file_path. 默认生成临时文件
 ### 可以用列表为每一列指定宽度 col_width
 ### 指定字体大小 font_size
 path = ds.to_image(df, file_path=None, col_width=None, font_size=None)
 ```
 
+#### 常用模型
+
+```python
+from pyqueen import Model
+
+data = df['待预测列']  # 也可以是 list形式的数据
+### forecast_step: 预测节点数
+### p,d,q: 自定义arima模型参数. 为空时自动使用最优模型
+forecast_result = Model.arima(data, forecast_step=10, p=None, d=None, q=None)
+```
 #### ETL辅助功能
+
 ```python
 # 使用SQL语法查询 pd.DataFrame 数据 (功能依赖duckdb包); 可以部分代替 pandas接口 
 ### 等价python
 df_fact = pd.merge(df_fact, df_dim1, on='d1', how='inner')
 df_fact = pd.merge(df_fact, df_dim1, on='d2', how='inner')
-df_summary = df_fact.groupby(['d1_name','d2_name']).agg({'value':np.sum}).reset_index().rename('value':'sum_value')
+df_summary = df_fact.groupby(['d1_name', 'd2_name']).agg({'value': np.sum}).reset_index().rename('value':'sum_value')
 
 ### 可以用sql实现
 from pyqueen import DataSource
+
 ds = DataSource()
 data = {'table1': df_fact, 'table2': df_dim1, 'table3': df_dim2}
 sql = '''
   select b.d1_name,c.d2_name,sum(a.value) as sum_value
   from table1 a 
   inner join table2 b on a.d1 = b.d1
   inner join table3 c on a.d2 = c.d2
   group by b.d1_name,c.d2_name
 '''
 df_summary = ds.pdsql(sql=sql, data=data)
 
-
 # 导入测试数据
 ### 会将excel文件里的每一个sheet映射成一张表, 将这个 ds 后续的sql查询都转移到这个由excel文件生成的新数据库
 ### 用于测试确认复杂计算逻辑, 相当于用excel文件代替测试数据库
 ds.import_test_data(excel_path='')
 ```
 
-
 #### 下载FTP文件
 
 ```python
 from pyqueen import DataSource
 
 ds = DataSource(host='', username='', password='', port='', db_type='ftp')
 ds.download_ftp(local_dir='保存目录', remote_dir='远程目录')
 ```
 
 #### 写入Excel文件
+
 - 将 pd.DataFrame对象 写入Excel文件
 - file_path 文件路径 (须以 .xlsx 结尾)
 - sheet_list 待写入数据, 二维列表, 每个 pd.DataFrame对象 对应一个 sheet
 - fillna='' 空值填充
 - fmt=None 字段格式,可以按字段名指定
 - font='微软雅黑' 字体
 - font_color='black' 字体颜色
@@ -122,39 +157,40 @@
     'col4': '0.00%',
     'col5': 'YYYY-MM-DD'
 }
 ds.to_excel(file_path='xxx.xlsx', sheet_list=sheet_list, fmt=fmt)
 ```
 
 #### 时间处理工具
+
 ```python
 from pyqueen import TimeKit
 
 # 按当前时间
 tk = TimeKit()
 # 指定日期, 时间
 tk = TimeKit(theday=20200101, thetime=120000)
 
 # 常用属性
-tk.today    # 当前日期或初始化指定日期
-tk.now    # 当前时间或初始化指定时间
-tk.hour    # 当前小时
-tk.minute    # 当前分钟
-tk.second    # 当前秒
-tk.nday_of_week    # 1-7对应周一到周日
-tk.week_start    # 本周一日期
-tk.lw_start    # 上周开始日期
-tk.lw_end    # 上周结束日期
-tk.lw2_start    # 上上周开始日期
-tk.lw2_end    # 上上周结束日期
-tk.month_start    # 本月初
-tk.lm_start    # 上月初
-tk.lm_end    # 上月末
-tk.lm2_start    # 上上月初
-tk.lm2_end    # 上上月末
+tk.today  # 当前日期或初始化指定日期
+tk.now  # 当前时间或初始化指定时间
+tk.hour  # 当前小时
+tk.minute  # 当前分钟
+tk.second  # 当前秒
+tk.nday_of_week  # 1-7对应周一到周日
+tk.week_start  # 本周一日期
+tk.lw_start  # 上周开始日期
+tk.lw_end  # 上周结束日期
+tk.lw2_start  # 上上周开始日期
+tk.lw2_end  # 上上周结束日期
+tk.month_start  # 本月初
+tk.lm_start  # 上月初
+tk.lm_end  # 上月末
+tk.lm2_start  # 上上月初
+tk.lm2_end  # 上上月末
 
 # 时间加减
 # flag: 加减单位: years,months,days,hours,minutes,seconds
 # value: 加减值
 # thetime之前 value 写负值
 # thetime之后 value 写正值
 new_day = tk.time_delta('20230101', 'days', -30)
@@ -170,14 +206,15 @@
 # 查询任意日期是星期几
 n = tk.get_nday_of_week(20200101)
 # 数值型日期转字符串
 date_str = tk.int2str(20200101, sep='-')
 ```
 
 #### ETL日志
+
 - 记录所有 `DataSource` 类函数的调用过程和相应参数
 - 如需启用日志, 添加: `ds.set_logger(logger)`
 - 其中 `logger` 为日志处理函数, 默认为: `print`
 - 自定义 `logger` 参考 `example/etl_with_log.py`
 - `etl_log` 所有 **key**
     - py_path: 调用脚本路径
     - func_name: 调用函数名
@@ -190,14 +227,15 @@
     - host: (如有) 服务器地址
     - db_type: (如有) 数据库类型
     - port: (如有) 端口
     - db_name: (如有) 数据库名
     - table_name: (如有) 表名
 
 #### 发送信息
+
 - 邮件
 - 钉钉
 - 企业微信
 
 ```python
 from pyqueen import Email
 
@@ -238,14 +276,15 @@
 # content不为None时,发送文本
 # mentioned_list: userid的列表，提醒群中的指定成员(@某个成员)，@all表示提醒所有人
 # mentioned_mobile_list: 手机号列表，提醒手机号对应的群成员(@某个成员)，@all表示提醒所有人
 wechat.send(content=None, mentioned_list=None, mentioned_mobile_list=None)
 ```
 
 #### 小工具
+
 ```python
 from pyqueen import Utils
 
 # 压缩/解压缩
 Utils.zip(from_path='', to_path='')
 Utils.unzip(from_path='', to_path='')
 # 删除文件
@@ -264,18 +303,19 @@
 ### args_list: 每个子任务的参数
 ### max_process = 1: 最大进程数, 默认为 1
 ### 以list返回每个子进程执行结果, 和 args_list 顺序一致
 result = Utils.mult_run(func, args_list=[], max_process=1)
 ```
 
 #### 命令行
+
 ```commandline
 用法: pyqueen command args1,args2,...
 ---
 command: 
     #1  sql2table [file_path] 从sql解析用到的表(通过正则解析, 有误差) (不带参数时读取剪切板)
     
-    #2  getcode file_path: 检测文件编码
+    #2  detcode file_path: 检测文件编码
     
-    #3 md5 基于剪切板文本生成md5
+    #3  md5 基于剪切板文本生成md5
 ```
```

### Comparing `pyqueen-1.0.8/pyqueen/etl/data_source.py` & `pyqueen-1.0.9/pyqueen/io/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import pandas as pd
-from pyqueen.etl.excel import Excel
+from pyqueen.io.excel import Excel
 
 
 class DataSource:
     def __init__(self, host=None, username=None, password=None, port=None, db_name=None, db_type='MySQL'):
         if str(db_type).lower() in ('mysql', 'mssql', 'oracle', 'clickhouse', 'sqlite'):
-            from pyqueen.etl.db import DB
+            from pyqueen.io.db import DB
             self.__db = DB(host=host, username=username, password=password, port=port, db_name=db_name, db_type=db_type)
         if str(db_type).lower() == 'ftp':
             from ftp import FTP
             self.__ftp = FTP(username=username, password=password, host=host, port=port)
         self.__excel = Excel()
         self.__logger = None
         self.__host = host
@@ -32,28 +32,28 @@
             'db_type',
             'port',
             'db_name',
             'table_name'
         ]
 
     def import_test_data(self, excel_path):
-        from pyqueen.etl.db import DB
+        from pyqueen.io.db import DB
         self.__db = DB(host=':memory:', db_name='main', db_type='sqlite')
         self.__db.keep_conn()
         data = pd.read_excel(excel_path, sheet_name=None)
         for sht_name, df in data.items():
             self.__db.to_db(df, sht_name)
 
     @staticmethod
     def __file_log(etl_log):
         log_path = etl_log['py_path']
         log_path = str(log_path).replace('.py', '.log')
         info = '\n------------------------------------\n'
         for k, v in etl_log.items():
-            info += '    ' + str(k) + ': ' + str(v) + '\n'
+            info += str(k) + ': ' + str(v) + '\n'
         info += '\n------------------------------------\n'
         with open(log_path, 'a+', encoding='utf-8') as f:
             f.write(info)
 
     def set_logger(self, logger=print):
         if str(logger) == 'file':
             self.__logger = self.__file_log
@@ -258,10 +258,10 @@
             for df_name, df in data.items():
                 conn.register(df_name, df)
             result = conn.execute(sql).df()
         return result
 
     @staticmethod
     def to_image(df, file_path=None, col_width=None, font_size=None):
-        from pyqueen.etl.image import Image
+        from pyqueen.io.image import Image
         path = Image.df2image(df, file_path=file_path, col_width=col_width, font_size=font_size)
         return path
```

### Comparing `pyqueen-1.0.8/pyqueen/etl/db.py` & `pyqueen-1.0.9/pyqueen/io/db.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/etl/excel.py` & `pyqueen-1.0.9/pyqueen/io/excel.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/etl/ftp.py` & `pyqueen-1.0.9/pyqueen/io/ftp.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/etl/image.py` & `pyqueen-1.0.9/pyqueen/io/image.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/service/pydingtalk.py` & `pyqueen-1.0.9/pyqueen/service/pydingtalk.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/service/pyemail.py` & `pyqueen-1.0.9/pyqueen/service/pyemail.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/service/pywechat.py` & `pyqueen-1.0.9/pyqueen/service/pywechat.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/service/showdoc.py` & `pyqueen-1.0.9/pyqueen/service/showdoc.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/utility/command.py` & `pyqueen-1.0.9/pyqueen/utility/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,17 @@
         |___/                                                                               
 =================================================================================                                                                                              
 用法: pyqueen command args1,args2,...
 ---
 command: 
     #1  sql2table [file_path] 从sql解析用到的表(通过正则解析, 有误差) (不带参数时读取剪切板)
     
-    #2  getcode file_path 检测文件编码
+    #2  detcode file_path 检测文件编码
     
-    #3 md5 基于剪切板文本生成md5
+    #3  md5 基于剪切板文本生成md5
 '''
 
 
 def cmd():
     parms = sys.argv[1:]
     if len(parms) == 0:
         print(doc)
@@ -33,21 +33,23 @@
             with open(parms[1], 'r', encoding='utf-8') as f:
                 sql_text = f.read()
         tb_list = Utils.sql2table(sql_text)
         print('================= begin =========================\n')
         for tb in tb_list:
             print(tb)
         print('\n================= end =========================\n')
-    elif parms[0] == 'getcode':
+    elif parms[0] == 'detcode':
         if len(parms) >= 2:
             print('================= begin =========================\n')
             encoding, confidence = Utils.detect_encoding(parms[1])
+            confidence = str(int(confidence * 100)) + '%'
             print('文件编码: %s, 可信度: %s' % (str(encoding), str(confidence)))
             print('\n================= end =========================\n')
         else:
             print('指定文件路径')
     elif parms[0] == 'md5':
         import pyperclip
         text = str(pyperclip.paste()).replace('\n', '').strip(' ')
         print('================= begin =========================\n')
+        print('输入文本: "%s"\n' % text)
         print(Utils.md5(text))
         print('\n================= end =========================\n')
```

### Comparing `pyqueen-1.0.8/pyqueen/utility/time_kit.py` & `pyqueen-1.0.9/pyqueen/utility/time_kit.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen/utility/utils.py` & `pyqueen-1.0.9/pyqueen/utility/utils.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.0.8/pyqueen.egg-info/PKG-INFO` & `pyqueen-1.0.9/pyqueen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqueen
-Version: 1.0.8
+Version: 1.0.9
 Summary: Rule your Data
 Home-page: https://github.com/ts7ming/pyqueen.git
 Author: ts7ming
 Author-email: qiming.ma@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,46 +14,51 @@
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: SQLAlchemy==1.4.49
 Requires-Dist: xlrd==1.2.0
 Requires-Dist: XlsxWriter
 
 # PyQueen
+
 ![](logo.jpg)
 
 ![github license](https://img.shields.io/github/license/ts7ming/pyqueen)
 [![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)
 ![Language](https://img.shields.io/badge/language-Python-brightgreen)
 [![Documentation Status](https://readthedocs.org/projects/pyqueen/badge/?version=latest)](https://pyqueen.readthedocs.io/zh-cn/latest/?badge=latest)
 ![GitHub Repo stars](https://img.shields.io/github/stars/ts7ming/pyqueen)
+[![PyPI downloads](https://img.shields.io/pypi/dm/pyqueen.svg)](https://pypistats.org/packages/pyqueen)
 
-PyQueen 是一个简单的数据处理工具箱. 配合 Pandas 使用可以完成简单的ETL作业
+PyQueen 是一个数据处理工具箱. 配合 Pandas 使用可以完成简单的ETL作业
 
 ## Install
+
 ```bash
 pip install pyqueen
 ```
 
 ## Doc
+
 - [readthedocs](https://pyqueen.readthedocs.io/zh-cn/latest/)
 - 示例: example/*
 
 #### 读写数据库
+
 - dbtype: 可选 mysql,mssql,oracle,clickhouse,sqlite
 - 每次操作数据库都会销毁连接, 无需关注连接池情况
-  - 如需主动控制连接 使用: `ds.keep_conn()` 和 `ds.close_conn()`
+    - 如需主动控制连接 使用: `ds.keep_conn()` 和 `ds.close_conn()`
 - 如需切换 db_name 使用: `ds.set_db(db_name)`
 - 设置字符集 使用: `ds.set_charset(charset)`. 默认: `utf8mb4`
 - 设置 chunksize 使用 `ds.set_chunksize(1000)`. 默认: `10000`
 - 数据库连接支持
-  - mysql: `pip install pymysql`
-  - mssql: `pip install pymssql` 
-    - 可选 `pip install pyodbc` 需指定 `ds.set_package('pyodbc')`
-  - oracle: `pip install cx_oracle`
-  - clickhouse: `pip install clickhouse-driver`
+    - mysql: `pip install pymysql`
+    - mssql: `pip install pymssql`
+        - 可选 `pip install pyodbc` 需指定 `ds.set_package('pyodbc')`
+    - oracle: `pip install cx_oracle`
+    - clickhouse: `pip install clickhouse-driver`
 
 ```python
 from pyqueen import DataSource
 
 ds = DataSource(host='', username='', password='', port='', db_name='', db_type='')
 
 # 根据sql查询, 返回 pd.DataFrame 对象
@@ -72,53 +77,64 @@
 # pd.DataFrame 转图片
 ### 可以指定文件路径: file_path. 默认生成临时文件
 ### 可以用列表为每一列指定宽度 col_width
 ### 指定字体大小 font_size
 path = ds.to_image(df, file_path=None, col_width=None, font_size=None)
 ```
 
+#### 常用模型
+
+```python
+from pyqueen import Model
+
+data = df['待预测列']  # 也可以是 list形式的数据
+### forecast_step: 预测节点数
+### p,d,q: 自定义arima模型参数. 为空时自动使用最优模型
+forecast_result = Model.arima(data, forecast_step=10, p=None, d=None, q=None)
+```
 #### ETL辅助功能
+
 ```python
 # 使用SQL语法查询 pd.DataFrame 数据 (功能依赖duckdb包); 可以部分代替 pandas接口 
 ### 等价python
 df_fact = pd.merge(df_fact, df_dim1, on='d1', how='inner')
 df_fact = pd.merge(df_fact, df_dim1, on='d2', how='inner')
-df_summary = df_fact.groupby(['d1_name','d2_name']).agg({'value':np.sum}).reset_index().rename('value':'sum_value')
+df_summary = df_fact.groupby(['d1_name', 'd2_name']).agg({'value': np.sum}).reset_index().rename('value':'sum_value')
 
 ### 可以用sql实现
 from pyqueen import DataSource
+
 ds = DataSource()
 data = {'table1': df_fact, 'table2': df_dim1, 'table3': df_dim2}
 sql = '''
   select b.d1_name,c.d2_name,sum(a.value) as sum_value
   from table1 a 
   inner join table2 b on a.d1 = b.d1
   inner join table3 c on a.d2 = c.d2
   group by b.d1_name,c.d2_name
 '''
 df_summary = ds.pdsql(sql=sql, data=data)
 
-
 # 导入测试数据
 ### 会将excel文件里的每一个sheet映射成一张表, 将这个 ds 后续的sql查询都转移到这个由excel文件生成的新数据库
 ### 用于测试确认复杂计算逻辑, 相当于用excel文件代替测试数据库
 ds.import_test_data(excel_path='')
 ```
 
-
 #### 下载FTP文件
 
 ```python
 from pyqueen import DataSource
 
 ds = DataSource(host='', username='', password='', port='', db_type='ftp')
 ds.download_ftp(local_dir='保存目录', remote_dir='远程目录')
 ```
 
 #### 写入Excel文件
+
 - 将 pd.DataFrame对象 写入Excel文件
 - file_path 文件路径 (须以 .xlsx 结尾)
 - sheet_list 待写入数据, 二维列表, 每个 pd.DataFrame对象 对应一个 sheet
 - fillna='' 空值填充
 - fmt=None 字段格式,可以按字段名指定
 - font='微软雅黑' 字体
 - font_color='black' 字体颜色
@@ -141,39 +157,40 @@
     'col4': '0.00%',
     'col5': 'YYYY-MM-DD'
 }
 ds.to_excel(file_path='xxx.xlsx', sheet_list=sheet_list, fmt=fmt)
 ```
 
 #### 时间处理工具
+
 ```python
 from pyqueen import TimeKit
 
 # 按当前时间
 tk = TimeKit()
 # 指定日期, 时间
 tk = TimeKit(theday=20200101, thetime=120000)
 
 # 常用属性
-tk.today    # 当前日期或初始化指定日期
-tk.now    # 当前时间或初始化指定时间
-tk.hour    # 当前小时
-tk.minute    # 当前分钟
-tk.second    # 当前秒
-tk.nday_of_week    # 1-7对应周一到周日
-tk.week_start    # 本周一日期
-tk.lw_start    # 上周开始日期
-tk.lw_end    # 上周结束日期
-tk.lw2_start    # 上上周开始日期
-tk.lw2_end    # 上上周结束日期
-tk.month_start    # 本月初
-tk.lm_start    # 上月初
-tk.lm_end    # 上月末
-tk.lm2_start    # 上上月初
-tk.lm2_end    # 上上月末
+tk.today  # 当前日期或初始化指定日期
+tk.now  # 当前时间或初始化指定时间
+tk.hour  # 当前小时
+tk.minute  # 当前分钟
+tk.second  # 当前秒
+tk.nday_of_week  # 1-7对应周一到周日
+tk.week_start  # 本周一日期
+tk.lw_start  # 上周开始日期
+tk.lw_end  # 上周结束日期
+tk.lw2_start  # 上上周开始日期
+tk.lw2_end  # 上上周结束日期
+tk.month_start  # 本月初
+tk.lm_start  # 上月初
+tk.lm_end  # 上月末
+tk.lm2_start  # 上上月初
+tk.lm2_end  # 上上月末
 
 # 时间加减
 # flag: 加减单位: years,months,days,hours,minutes,seconds
 # value: 加减值
 # thetime之前 value 写负值
 # thetime之后 value 写正值
 new_day = tk.time_delta('20230101', 'days', -30)
@@ -189,14 +206,15 @@
 # 查询任意日期是星期几
 n = tk.get_nday_of_week(20200101)
 # 数值型日期转字符串
 date_str = tk.int2str(20200101, sep='-')
 ```
 
 #### ETL日志
+
 - 记录所有 `DataSource` 类函数的调用过程和相应参数
 - 如需启用日志, 添加: `ds.set_logger(logger)`
 - 其中 `logger` 为日志处理函数, 默认为: `print`
 - 自定义 `logger` 参考 `example/etl_with_log.py`
 - `etl_log` 所有 **key**
     - py_path: 调用脚本路径
     - func_name: 调用函数名
@@ -209,14 +227,15 @@
     - host: (如有) 服务器地址
     - db_type: (如有) 数据库类型
     - port: (如有) 端口
     - db_name: (如有) 数据库名
     - table_name: (如有) 表名
 
 #### 发送信息
+
 - 邮件
 - 钉钉
 - 企业微信
 
 ```python
 from pyqueen import Email
 
@@ -257,14 +276,15 @@
 # content不为None时,发送文本
 # mentioned_list: userid的列表，提醒群中的指定成员(@某个成员)，@all表示提醒所有人
 # mentioned_mobile_list: 手机号列表，提醒手机号对应的群成员(@某个成员)，@all表示提醒所有人
 wechat.send(content=None, mentioned_list=None, mentioned_mobile_list=None)
 ```
 
 #### 小工具
+
 ```python
 from pyqueen import Utils
 
 # 压缩/解压缩
 Utils.zip(from_path='', to_path='')
 Utils.unzip(from_path='', to_path='')
 # 删除文件
@@ -283,18 +303,19 @@
 ### args_list: 每个子任务的参数
 ### max_process = 1: 最大进程数, 默认为 1
 ### 以list返回每个子进程执行结果, 和 args_list 顺序一致
 result = Utils.mult_run(func, args_list=[], max_process=1)
 ```
 
 #### 命令行
+
 ```commandline
 用法: pyqueen command args1,args2,...
 ---
 command: 
     #1  sql2table [file_path] 从sql解析用到的表(通过正则解析, 有误差) (不带参数时读取剪切板)
     
-    #2  getcode file_path: 检测文件编码
+    #2  detcode file_path: 检测文件编码
     
-    #3 md5 基于剪切板文本生成md5
+    #3  md5 基于剪切板文本生成md5
 ```
```

### Comparing `pyqueen-1.0.8/pyqueen.egg-info/SOURCES.txt` & `pyqueen-1.0.9/pyqueen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 pyqueen/__init__.py
 pyqueen.egg-info/PKG-INFO
 pyqueen.egg-info/SOURCES.txt
 pyqueen.egg-info/dependency_links.txt
 pyqueen.egg-info/entry_points.txt
 pyqueen.egg-info/requires.txt
 pyqueen.egg-info/top_level.txt
-pyqueen/etl/__init__.py
-pyqueen/etl/data_source.py
-pyqueen/etl/db.py
-pyqueen/etl/excel.py
-pyqueen/etl/ftp.py
-pyqueen/etl/image.py
+pyqueen/analysis/__init__.py
+pyqueen/analysis/model.py
+pyqueen/io/__init__.py
+pyqueen/io/data_source.py
+pyqueen/io/db.py
+pyqueen/io/excel.py
+pyqueen/io/ftp.py
+pyqueen/io/image.py
 pyqueen/service/__init__.py
 pyqueen/service/pydingtalk.py
 pyqueen/service/pyemail.py
 pyqueen/service/pywechat.py
 pyqueen/service/showdoc.py
 pyqueen/utility/__init__.py
 pyqueen/utility/command.py
```

### Comparing `pyqueen-1.0.8/setup.py` & `pyqueen-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyqueen',
-    version='1.0.8',
+    version='1.0.9',
     url='https://github.com/ts7ming/pyqueen.git',
     description='Rule your Data',
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author='ts7ming',
     author_email='qiming.ma@outlook.com',
     packages=find_packages(),
```

