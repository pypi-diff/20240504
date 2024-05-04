# Comparing `tmp/lab_student_survey-0.4.8.tar.gz` & `tmp/lab_student_survey-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab_student_survey-0.4.8.tar", max compression
+gzip compressed data, was "lab_student_survey-0.4.9.tar", max compression
```

## Comparing `lab_student_survey-0.4.8.tar` & `lab_student_survey-0.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/LICENSE
--rw-r--r--   0        0        0     7220 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/README.md
--rw-r--r--   0        0        0     2795 2023-11-13 04:43:35.886608 lab_student_survey-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/src/lab_student_survey/__init__.py
--rw-r--r--   0        0        0       59 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/src/lab_student_survey/__main__.py
--rw-r--r--   0        0        0    13922 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/src/lab_student_survey/analyze.py
--rw-r--r--   0        0        0     1295 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/src/lab_student_survey/cli.py
--rw-r--r--   0        0        0     1290 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/src/lab_student_survey/gdrive.py
--rw-r--r--   0        0        0     2574 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/src/lab_student_survey/main.py
--rw-r--r--   0        0        0        0 2023-11-13 04:43:24.530597 lab_student_survey-0.4.8/src/lab_student_survey/py.typed
--rw-r--r--   0        0        0     8768 1970-01-01 00:00:00.000000 lab_student_survey-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/LICENSE
+-rw-r--r--   0        0        0     7340 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/README.md
+-rw-r--r--   0        0        0     2795 2023-11-30 02:46:06.392078 lab_student_survey-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/src/lab_student_survey/__init__.py
+-rw-r--r--   0        0        0       59 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/src/lab_student_survey/__main__.py
+-rw-r--r--   0        0        0    14265 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/src/lab_student_survey/analyze.py
+-rw-r--r--   0        0        0     1295 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/src/lab_student_survey/cli.py
+-rw-r--r--   0        0        0     1290 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/src/lab_student_survey/gdrive.py
+-rw-r--r--   0        0        0     2574 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/src/lab_student_survey/main.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:45:58.228004 lab_student_survey-0.4.9/src/lab_student_survey/py.typed
+-rw-r--r--   0        0        0     8888 1970-01-01 00:00:00.000000 lab_student_survey-0.4.9/PKG-INFO
```

### Comparing `lab_student_survey-0.4.8/LICENSE` & `lab_student_survey-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lab_student_survey-0.4.8/README.md` & `lab_student_survey-0.4.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,21 +60,25 @@
 ### Github Actions
 
 ```yaml
 name: Run lab-student-survey
 
 on:
   schedule:
-    - cron: "0 * * * *" # every hour
+    # every day at 00:00 UTC
+    - cron: "0 0 * * *"
+  workflow_dispatch:
 
 jobs:
   run:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
+      - name: Install wkhtmltopdf
+        run: sudo apt-get install -y wkhtmltopdf
       - name: Install and run lab-student-survey
         run: pipx run lab-student-survey
         env:
           LAB_STUDENT_SURVEY_FILE_URL: ${{ secrets.LAB_STUDENT_SURVEY_FILE_URL }}
           LAB_STUDENT_SURVEY_FOLDER_URL: ${{ secrets.LAB_STUDENT_SURVEY_FOLDER_URL }}
           GDRIVE_SERVICE_SECRETS: ${{ secrets.GDRIVE_SERVICE_SECRETS }}
 ```
```

#### html2text {}

```diff
@@ -21,26 +21,28 @@
 Variables - Set the `Google Sheet` ID as `LAB_STUDENT_SURVEY_FILE_ID`
 environment variable (via GitHub Secrets). - Set the `student-lab-survey`
 folder ID as `LAB_STUDENT_SURVEY_FOLDER_ID` environment variable (via GitHub
 Secrets). (Optional.) If not set, the parent folder ID of the `Google Sheet`
 will be used. - (Set the `Service Account` credentials as
 `GDRIVE_SERVICE_ACCOUNT` environment variable (via GitHub Secrets).) ###
 Running commands ```shell lss ``` ### Github Actions ```yaml name: Run lab-
-student-survey on: schedule: - cron: "0 * * * *" # every hour jobs: run: runs-
-on: ubuntu-latest steps: - uses: actions/checkout@v3 - name: Install and run
-lab-student-survey run: pipx run lab-student-survey env:
-LAB_STUDENT_SURVEY_FILE_URL: ${{ secrets.LAB_STUDENT_SURVEY_FILE_URL }}
-LAB_STUDENT_SURVEY_FOLDER_URL: ${{ secrets.LAB_STUDENT_SURVEY_FOLDER_URL }}
-GDRIVE_SERVICE_SECRETS: ${{ secrets.GDRIVE_SERVICE_SECRETS }} ``` ##
-Installation Install this via pip or pipx (or your favourite package manager):
-```shell pipx install lab-student-survey ``` ## Alternatives As far as I could
-find, there is no repository on GitHub for this particular topic. Instead, you
-may want to check out the following alternative websites. However, as there are
-too few people in a lab, with the effect of diminishing anonymity, most of
-these websites do not seem to attract many reviews. ### å½å -
+student-survey on: schedule: # every day at 00:00 UTC - cron: "0 0 * * *"
+workflow_dispatch: jobs: run: runs-on: ubuntu-latest steps: - uses: actions/
+checkout@v3 - name: Install wkhtmltopdf run: sudo apt-get install -
+y wkhtmltopdf - name: Install and run lab-student-survey run: pipx run lab-
+student-survey env: LAB_STUDENT_SURVEY_FILE_URL: ${
+{ secrets.LAB_STUDENT_SURVEY_FILE_URL }} LAB_STUDENT_SURVEY_FOLDER_URL: ${
+{ secrets.LAB_STUDENT_SURVEY_FOLDER_URL }} GDRIVE_SERVICE_SECRETS: ${
+{ secrets.GDRIVE_SERVICE_SECRETS }} ``` ## Installation Install this via pip or
+pipx (or your favourite package manager): ```shell pipx install lab-student-
+survey ``` ## Alternatives As far as I could find, there is no repository on
+GitHub for this particular topic. Instead, you may want to check out the
+following alternative websites. However, as there are too few people in a lab,
+with the effect of diminishing anonymity, most of these websites do not seem to
+attract many reviews. ### å½å -
 [çç³»ç ç©¶å®¤ã®ã¯ãã³ããµã¤ãï½OpenLab](https://openlabmg.com/):
 **åéåæ­¢ä¸­**,
 æç¨¿ããã¨Amazonã®ããå¸ï¼100åï¼ããããã,
 ã»ã¨ãã©æå ±ãªã(100ç¨åº¦?) - [LabBase ç ç©¶å®¤ãµã¼ã](https://
 lab-search.app.labbase.jp/): **å¥åæ¹æ³ä¸æ**, ä¸ãããæå ±ãªã -
 [ç ç©¶å®¤ãã](http://kenkyu-navi.com): ãªã³ã¯åã [Forms](https://
 docs.google.com/forms/d/1s-c8tGOCGLv35KimBo9U7d3MKPyXpDl_QcHLozppAgM/
```

### Comparing `lab_student_survey-0.4.8/pyproject.toml` & `lab_student_survey-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lab-student-survey"
-version = "0.4.8"
+version = "0.4.9"
 description = "Python package for lab student survey"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/lab-student-survey"
 documentation = "https://lab-student-survey.readthedocs.io"
 classifiers = [
```

### Comparing `lab_student_survey-0.4.8/src/lab_student_survey/analyze.py` & `lab_student_survey-0.4.9/src/lab_student_survey/analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,15 +233,16 @@
     )
     df_likert_mean.sort_index(axis=0, inplace=False, ascending=False).drop(
         columns=list(df_numeral_columns) + ["mean"], inplace=False
     ).plot(kind="barh", ax=ax[1], stacked=True)
     # sns.barplot(df_likert_mean, orient="h", ax=ax[1])
 
     # calculate corr
-    if len(df_likert_mean) == 1:
+    print(df_likert_mean)
+    if len(df_likert_mean) < 2:
         df_likert_mean_corr = pd.DataFrame()
         fig_corr = plt.figure()
         df_likert_mean_pval = pd.DataFrame()
         df_likert_std = pd.DataFrame()
         df_likert_colwise = pd.DataFrame()
         fig_colwise = plt.figure()
     else:
@@ -252,16 +253,23 @@
             fig_corr_dropped, ax_corr_dropped = plt.subplots(figsize=(10, 10))
             df_corr_dropped = df_likert_mean_corr.drop(
                 index=df_numeral_columns, columns=df_numeral_columns
             )
             sns.heatmap(df_corr_dropped, annot=True, ax=ax_corr_dropped)
 
         # calculate p-values
+        def try_peasonr(x: pd.Series, y: pd.Series) -> float:
+            try:
+                return pearsonr(x, y)[1]
+            except Exception as e:
+                LOG.warning(e)
+                return float("nan")
+
         df_likert_mean_pval = df_likert_mean.corr(
-            method=lambda x, y: pearsonr(x, y)[1]
+            method=lambda x, y: try_peasonr(x, y)
         ) - np.eye(len(df_likert_mean_corr))
 
         # calculate mean and std for each column
         df_likert_grouped_colwise = df_likert.T.groupby(
             level="group", axis=0, sort=False
         )
         df_liekrt_mean_colwise = (
@@ -295,15 +303,18 @@
             #     0.5: "<span style='color: #007700'>Poor</span>",
             #     float("-inf"): "<span style='color: #005500'>Unacceptable</span>"
             # }
             return {
                 "alpha": a[0],
                 "alpha_0.95": a[1],
                 "internal_consistency": internal_consistency[
-                    max(filter(lambda x: x <= a[0], internal_consistency.keys()))
+                    max(
+                        list(filter(lambda x: x <= a[0], internal_consistency.keys()))
+                        or [float("-inf")]
+                    )
                 ],
             }
 
         df_likert_alpha = df_likert_grouped.apply(
             lambda x: _parse_cronbach_alpha(x)
         ).apply(pd.Series)
         df_likert_colwise = pd.concat(
```

### Comparing `lab_student_survey-0.4.8/src/lab_student_survey/cli.py` & `lab_student_survey-0.4.9/src/lab_student_survey/cli.py`

 * *Files identical despite different names*

### Comparing `lab_student_survey-0.4.8/src/lab_student_survey/gdrive.py` & `lab_student_survey-0.4.9/src/lab_student_survey/gdrive.py`

 * *Files identical despite different names*

### Comparing `lab_student_survey-0.4.8/src/lab_student_survey/main.py` & `lab_student_survey-0.4.9/src/lab_student_survey/main.py`

 * *Files identical despite different names*

### Comparing `lab_student_survey-0.4.8/PKG-INFO` & `lab_student_survey-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-student-survey
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python package for lab student survey
 Home-page: https://github.com/34j/lab-student-survey
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -96,21 +96,25 @@
 ### Github Actions
 
 ```yaml
 name: Run lab-student-survey
 
 on:
   schedule:
-    - cron: "0 * * * *" # every hour
+    # every day at 00:00 UTC
+    - cron: "0 0 * * *"
+  workflow_dispatch:
 
 jobs:
   run:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
+      - name: Install wkhtmltopdf
+        run: sudo apt-get install -y wkhtmltopdf
       - name: Install and run lab-student-survey
         run: pipx run lab-student-survey
         env:
           LAB_STUDENT_SURVEY_FILE_URL: ${{ secrets.LAB_STUDENT_SURVEY_FILE_URL }}
           LAB_STUDENT_SURVEY_FOLDER_URL: ${{ secrets.LAB_STUDENT_SURVEY_FOLDER_URL }}
           GDRIVE_SERVICE_SECRETS: ${{ secrets.GDRIVE_SERVICE_SECRETS }}
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lab-student-survey Version: 0.4.8 Summary: Python
+Metadata-Version: 2.1 Name: lab-student-survey Version: 0.4.9 Summary: Python
 package for lab student survey Home-page: https://github.com/34j/lab-student-
 survey License: MIT Author: 34j Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -41,26 +41,28 @@
 Variables - Set the `Google Sheet` ID as `LAB_STUDENT_SURVEY_FILE_ID`
 environment variable (via GitHub Secrets). - Set the `student-lab-survey`
 folder ID as `LAB_STUDENT_SURVEY_FOLDER_ID` environment variable (via GitHub
 Secrets). (Optional.) If not set, the parent folder ID of the `Google Sheet`
 will be used. - (Set the `Service Account` credentials as
 `GDRIVE_SERVICE_ACCOUNT` environment variable (via GitHub Secrets).) ###
 Running commands ```shell lss ``` ### Github Actions ```yaml name: Run lab-
-student-survey on: schedule: - cron: "0 * * * *" # every hour jobs: run: runs-
-on: ubuntu-latest steps: - uses: actions/checkout@v3 - name: Install and run
-lab-student-survey run: pipx run lab-student-survey env:
-LAB_STUDENT_SURVEY_FILE_URL: ${{ secrets.LAB_STUDENT_SURVEY_FILE_URL }}
-LAB_STUDENT_SURVEY_FOLDER_URL: ${{ secrets.LAB_STUDENT_SURVEY_FOLDER_URL }}
-GDRIVE_SERVICE_SECRETS: ${{ secrets.GDRIVE_SERVICE_SECRETS }} ``` ##
-Installation Install this via pip or pipx (or your favourite package manager):
-```shell pipx install lab-student-survey ``` ## Alternatives As far as I could
-find, there is no repository on GitHub for this particular topic. Instead, you
-may want to check out the following alternative websites. However, as there are
-too few people in a lab, with the effect of diminishing anonymity, most of
-these websites do not seem to attract many reviews. ### å½å -
+student-survey on: schedule: # every day at 00:00 UTC - cron: "0 0 * * *"
+workflow_dispatch: jobs: run: runs-on: ubuntu-latest steps: - uses: actions/
+checkout@v3 - name: Install wkhtmltopdf run: sudo apt-get install -
+y wkhtmltopdf - name: Install and run lab-student-survey run: pipx run lab-
+student-survey env: LAB_STUDENT_SURVEY_FILE_URL: ${
+{ secrets.LAB_STUDENT_SURVEY_FILE_URL }} LAB_STUDENT_SURVEY_FOLDER_URL: ${
+{ secrets.LAB_STUDENT_SURVEY_FOLDER_URL }} GDRIVE_SERVICE_SECRETS: ${
+{ secrets.GDRIVE_SERVICE_SECRETS }} ``` ## Installation Install this via pip or
+pipx (or your favourite package manager): ```shell pipx install lab-student-
+survey ``` ## Alternatives As far as I could find, there is no repository on
+GitHub for this particular topic. Instead, you may want to check out the
+following alternative websites. However, as there are too few people in a lab,
+with the effect of diminishing anonymity, most of these websites do not seem to
+attract many reviews. ### å½å -
 [çç³»ç ç©¶å®¤ã®ã¯ãã³ããµã¤ãï½OpenLab](https://openlabmg.com/):
 **åéåæ­¢ä¸­**,
 æç¨¿ããã¨Amazonã®ããå¸ï¼100åï¼ããããã,
 ã»ã¨ãã©æå ±ãªã(100ç¨åº¦?) - [LabBase ç ç©¶å®¤ãµã¼ã](https://
 lab-search.app.labbase.jp/): **å¥åæ¹æ³ä¸æ**, ä¸ãããæå ±ãªã -
 [ç ç©¶å®¤ãã](http://kenkyu-navi.com): ãªã³ã¯åã [Forms](https://
 docs.google.com/forms/d/1s-c8tGOCGLv35KimBo9U7d3MKPyXpDl_QcHLozppAgM/
```

