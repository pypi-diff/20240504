# Comparing `tmp/kmds-0.2.7.tar.gz` & `tmp/kmds-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmds-0.2.7.tar", max compression
+gzip compressed data, was "kmds-0.2.9.tar", max compression
```

## Comparing `kmds-0.2.7.tar` & `kmds-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     4401 2024-02-17 05:51:03.535725 kmds-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-02-05 02:47:21.294643 kmds-0.2.7/kmds/__init__.py
--rw-r--r--   0        0        0       41 2024-01-31 09:00:06.042893 kmds-0.2.7/kmds/config/kmds_app.yml
--rw-r--r--   0        0        0      711 2024-02-15 00:05:47.489689 kmds-0.2.7/kmds/examples/data_types_ITSM.csv
--rw-r--r--   0        0        0    25402 2024-02-16 06:31:59.189142 kmds-0.2.7/kmds/examples/example_analytics_kb_app_workflow.xml
--rw-r--r--   0        0        0   300319 2024-02-16 05:14:22.852174 kmds-0.2.7/kmds/examples/example_analytics_post_data_rep1_data.csv
--rw-r--r--   0        0        0   300319 2024-02-16 05:02:11.052973 kmds-0.2.7/kmds/examples/example_analytics_post_data_rep_data.csv
--rw-r--r--   0        0        0    17045 2024-02-16 04:03:31.833802 kmds-0.2.7/kmds/examples/example_ml_kb_exp_workflow.xml
--rw-r--r--   0        0        0 47106994 2023-11-03 01:13:00.260854 kmds-0.2.7/kmds/examples/incident_event_log_02.csv
--rw-r--r--   0        0        0   750404 2024-02-14 00:01:28.975543 kmds-0.2.7/kmds/examples/online_retail_Q1_2010.parquet
--rw-r--r--   0        0        0   226153 2024-02-16 05:00:16.707946 kmds-0.2.7/kmds/examples/q2_2016_ticket_resolution_data.csv
--rw-r--r--   0        0        0   528982 2024-02-14 00:01:28.955659 kmds-0.2.7/kmds/examples/retail_q1_post_EDA.parquet
--rw-r--r--   0        0        0  2174623 2024-02-14 00:01:28.972994 kmds-0.2.7/kmds/examples/retail_q1_post_data_rep_prep.parquet
--rw-r--r--   0        0        0   564995 2024-02-14 00:01:28.956930 kmds-0.2.7/kmds/examples/retail_q1_post_mc.parquet
--rw-r--r--   0        0        0  2174623 2024-02-14 00:01:29.023998 kmds-0.2.7/kmds/examples/retail_q1_sales_2010_summary.parquet
--rw-r--r--   0        0        0    22757 2024-02-17 03:27:03.808013 kmds-0.2.7/kmds/examples/test_kb_app_workflow
--rw-r--r--   0        0        0    19818 2024-02-14 00:01:29.024442 kmds-0.2.7/kmds/examples/test_kb_app_workflow.xml
--rw-r--r--   0        0        0    34663 2024-02-17 03:27:03.812296 kmds-0.2.7/kmds/examples/test_kb_exp_workflow
--rw-r--r--   0        0        0    28769 2024-02-14 00:01:28.954247 kmds-0.2.7/kmds/examples/test_kb_exp_workflow.xml
--rw-r--r--   0        0        0 14932161 2024-02-15 00:05:47.482790 kmds-0.2.7/kmds/examples/ticket_resolution_Q2_2016.csv
--rw-r--r--   0        0        0      102 2024-02-15 05:02:13.067379 kmds-0.2.7/kmds/examples/ticket_resolution_dtypes.csv
--rw-r--r--   0        0        0        0 2024-02-05 02:47:55.651819 kmds-0.2.7/kmds/ontology/__init__.py
--rw-r--r--   0        0        0    10002 2024-02-17 03:26:11.155574 kmds-0.2.7/kmds/ontology/kmds_ontology.py
--rw-r--r--   0        0        0     6788 2024-02-02 11:36:51.912776 kmds-0.2.7/kmds/ontology/kmds_ontology.xml
--rw-r--r--   0        0        0        0 2024-02-05 02:48:09.823356 kmds-0.2.7/kmds/pipelines/__init__.py
--rw-r--r--   0        0        0     3498 2024-01-30 01:47:03.403189 kmds-0.2.7/kmds/pipelines/retail_processing.py
--rw-r--r--   0        0        0        0 2024-02-05 02:48:20.877358 kmds-0.2.7/kmds/tagging/__init__.py
--rw-r--r--   0        0        0     1877 2024-02-14 03:39:05.870067 kmds-0.2.7/kmds/tagging/tag_types.py
--rw-r--r--   0        0        0        0 2024-02-05 02:48:45.866519 kmds-0.2.7/kmds/utils/__init__.py
--rw-r--r--   0        0        0      625 2024-02-07 08:41:02.201346 kmds-0.2.7/kmds/utils/config_reader.py
--rw-r--r--   0        0        0     4789 2024-02-16 22:57:27.309098 kmds-0.2.7/kmds/utils/load_utils.py
--rw-r--r--   0        0        0     1500 2024-02-14 13:33:52.064592 kmds-0.2.7/kmds/utils/path_utils.py
--rw-r--r--   0        0        0      658 2024-02-17 06:00:08.713624 kmds-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5238 1970-01-01 00:00:00.000000 kmds-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     4533 2024-02-23 07:00:27.867736 kmds-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-17 07:55:11.107408 kmds-0.2.9/kmds/__init__.py
+-rw-r--r--   0        0        0       41 2024-02-17 07:55:11.107929 kmds-0.2.9/kmds/config/kmds_app.yml
+-rw-r--r--   0        0        0      711 2024-02-17 07:55:11.108284 kmds-0.2.9/kmds/examples/data_types_ITSM.csv
+-rw-r--r--   0        0        0    25402 2024-02-17 07:55:11.108632 kmds-0.2.9/kmds/examples/example_analytics_kb_app_workflow.xml
+-rw-r--r--   0        0        0   300319 2024-02-17 07:55:11.109779 kmds-0.2.9/kmds/examples/example_analytics_post_data_rep1_data.csv
+-rw-r--r--   0        0        0   300319 2024-02-17 07:55:11.110340 kmds-0.2.9/kmds/examples/example_analytics_post_data_rep_data.csv
+-rw-r--r--   0        0        0    17700 2024-02-24 10:01:58.636791 kmds-0.2.9/kmds/examples/example_ml_kb_exp_workflow.xml
+-rw-r--r--   0        0        0 47106994 2024-02-17 07:55:11.161976 kmds-0.2.9/kmds/examples/incident_event_log_02.csv
+-rw-r--r--   0        0        0   750404 2024-02-17 07:55:11.166983 kmds-0.2.9/kmds/examples/online_retail_Q1_2010.parquet
+-rw-r--r--   0        0        0   226153 2024-02-17 07:55:11.167785 kmds-0.2.9/kmds/examples/q2_2016_ticket_resolution_data.csv
+-rw-r--r--   0        0        0   528982 2024-02-17 07:55:11.171318 kmds-0.2.9/kmds/examples/retail_q1_post_EDA.parquet
+-rw-r--r--   0        0        0  2174623 2024-02-17 07:55:11.175368 kmds-0.2.9/kmds/examples/retail_q1_post_data_rep_prep.parquet
+-rw-r--r--   0        0        0   564995 2024-02-17 07:55:11.177754 kmds-0.2.9/kmds/examples/retail_q1_post_mc.parquet
+-rw-r--r--   0        0        0  2174623 2024-02-17 07:55:11.180825 kmds-0.2.9/kmds/examples/retail_q1_sales_2010_summary.parquet
+-rw-r--r--   0        0        0   222756 2024-02-24 10:01:52.588868 kmds-0.2.9/kmds/examples/retail_transformed_q1_product_data.parquet
+-rw-r--r--   0        0        0    39462 2024-02-24 10:01:53.553688 kmds-0.2.9/kmds/examples/retail_transformed_q1_sales_data.parquet
+-rw-r--r--   0        0        0    22757 2024-02-17 07:55:11.181289 kmds-0.2.9/kmds/examples/test_kb_app_workflow
+-rw-r--r--   0        0        0    19818 2024-02-17 07:55:11.182723 kmds-0.2.9/kmds/examples/test_kb_app_workflow.xml
+-rw-r--r--   0        0        0    34663 2024-02-17 07:55:11.183438 kmds-0.2.9/kmds/examples/test_kb_exp_workflow
+-rw-r--r--   0        0        0    28769 2024-02-17 07:55:11.184287 kmds-0.2.9/kmds/examples/test_kb_exp_workflow.xml
+-rw-r--r--   0        0        0 14932161 2024-02-17 07:55:11.199103 kmds-0.2.9/kmds/examples/ticket_resolution_Q2_2016.csv
+-rw-r--r--   0        0        0      102 2024-02-17 07:55:11.199581 kmds-0.2.9/kmds/examples/ticket_resolution_dtypes.csv
+-rw-r--r--   0        0        0        0 2024-02-17 07:55:11.199623 kmds-0.2.9/kmds/ontology/__init__.py
+-rw-r--r--   0        0        0    10002 2024-02-17 07:55:11.200395 kmds-0.2.9/kmds/ontology/kmds_ontology.py
+-rw-r--r--   0        0        0     6788 2024-02-17 07:55:11.200789 kmds-0.2.9/kmds/ontology/kmds_ontology.xml
+-rw-r--r--   0        0        0        0 2024-02-17 07:55:11.200823 kmds-0.2.9/kmds/pipelines/__init__.py
+-rw-r--r--   0        0        0     3498 2024-02-17 07:55:11.201888 kmds-0.2.9/kmds/pipelines/retail_processing.py
+-rw-r--r--   0        0        0        0 2024-02-17 07:55:11.201923 kmds-0.2.9/kmds/tagging/__init__.py
+-rw-r--r--   0        0        0     1886 2024-02-26 15:19:26.891713 kmds-0.2.9/kmds/tagging/tag_types.py
+-rw-r--r--   0        0        0        0 2024-02-17 07:55:11.203388 kmds-0.2.9/kmds/utils/__init__.py
+-rw-r--r--   0        0        0      625 2024-02-17 07:55:11.203621 kmds-0.2.9/kmds/utils/config_reader.py
+-rw-r--r--   0        0        0     4789 2024-02-17 07:55:11.204308 kmds-0.2.9/kmds/utils/load_utils.py
+-rw-r--r--   0        0        0     1500 2024-02-17 07:55:11.204745 kmds-0.2.9/kmds/utils/path_utils.py
+-rw-r--r--   0        0        0      727 2024-02-27 03:18:54.111717 kmds-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 kmds-0.2.9/PKG-INFO
```

### Comparing `kmds-0.2.7/README.md` & `kmds-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+[![DOI](https://zenodo.org/badge/753950832.svg)](https://zenodo.org/doi/10.5281/zenodo.10695270)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 <p align="center">
   <img width="460" height="300" src="images/kmds_logo_resized.jpg">
 </p>
 
 ## Knowledge Management for Data Science
 
 ### What is this tool used for?
 
-This tool is used for knowledge management in data science. In software design, conceptual domain models inform lower-level models. In data science work, experiments yield knowledge that informs modeling choices. Data science models are almost always informed by a variety of analysis experiments. Experimentation and organization of knowledge artifacts supporting modeling decisions a requirement for reproducible data science models and improving model quality and performance.
+This tool is used for knowledge management in data science. In software design, conceptual domain models inform lower-level models. In data science work, experiments yield knowledge that informs modeling choices. Data science models are almost always informed by a variety of analysis experiments. Experimentation and organization of knowledge artifacts supporting modeling decisions is a requirement for reproducible data science models and improving model quality and performance.
 
 Please see [knowledge application development context](/feature_documentation/knowledge_management_in_DS.md ) for a description of a typical knowledge application development setting.
 
 ### Why do you need this tool?
 
-The above narrative suggests that ability to retrieve knowledge about experiments and historical models in an adhoc manner is critical in data science. It is. It is also grossly underserved. Knowledge management tools for domain specific models exist, knowledge management tools for dev-ops and ML-Ops exist, but tools for analytics and model development are siloed. Information gets fragmented over time. So analysts and data scientists often have to go to experiment tools, data catalogs or ML-Ops tools to fetch information they need to develop a model. In a subsequent iteration of this model, the contextual information that informed the development of this model if often lost and the development team, possibly with new team members, have the task of reconstructing this contextual information again. This library is a step in fixing this problem. The central idea is to organize tasks in terms of a sequence of steps that are pretty standard in data analysis work and capture knowledge in context while these tasks are performed.
+The above narrative suggests that ability to retrieve knowledge about experiments and historical models in an adhoc manner is critical in data science. It is. It is also grossly underserved. Knowledge management tools for domain specific models exist, knowledge management tools for dev-ops and ML-Ops exist, but tools for analytics and model development are siloed. Information gets fragmented over time. So analysts and data scientists often have to go to experiment tools, data catalogs or ML-Ops tools to fetch information they need to develop a model. In a subsequent iteration of this model, the contextual information that informed the development of this model is often lost, and the development team, possibly with new team members, have the task of reconstructing this contextual information again. This library is a step in fixing this problem. The central idea is to organize tasks in terms of a sequence of steps that are pretty standard in data analysis work and capture knowledge in context while these tasks are performed.
 
 ### How is it related to process guidelines and vocabularies for machine learning?
 Initiatives such as [CRISP DM](https://www.datascience-pm.com/crisp-dm-2/) provide guidelines and processes for developing data science projects. Projects such as [Open ML](https://openml.github.io/openml-python/main/index.html) provide semantic vocabulary standardization for machine learning tasks. These are excellent tools. However, the guidelines they provide are task focussed. The gap between a conceptual idea and the final, or, even candidate data science tasks for a project is filled with many assumptions and experimental evaluations. The information in these assumptions and experimental evaluations is what this tool aims to capture. There is also an ordering to these assumptions and experimental evaluations. This is also what this tool aims to capture.
 
 ### Who would use this tool?
 
 This tool is for data scientists and data analysts.
 
 ### How do you use this tool?
 
 1. You install this library along with the other python dependecies you need for your analysis task
 2. Review the [basic recipe](examples_of_use/workflow_recipe.md) for capturing your observations.
-3. Review [the templates section](examples_of_use/workflow_recipe.md) to find illustrative examples of the process to use this tool to capture knowledge facts in your data science workflows. For analytics projects, review the analytics template. For machine learning projects, review the machine learning template.
+3. Review [the templates section](examples_of_use/workflow_recipe.md) to find the example relevant to you. For analytics projects, review the analytics template. For machine learning projects, review the machine learning template.
 4. Start using the tool in your projects using the information from your review of the above two steps.
 
 ### Licensing and Feature Questions
 
 1. The tool is open source with an [apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0.txt)
 2. If you are interested in the following features, please set up a [meeting](https://calendly.com/rajiv-sambasivan/help-with-kmds-feature) with me:
    1. Help with a data analysis task for your use case
```

### Comparing `kmds-0.2.7/kmds/examples/data_types_ITSM.csv` & `kmds-0.2.9/kmds/examples/data_types_ITSM.csv`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/example_analytics_kb_app_workflow.xml` & `kmds-0.2.9/kmds/examples/example_analytics_kb_app_workflow.xml`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/example_analytics_post_data_rep1_data.csv` & `kmds-0.2.9/kmds/examples/example_analytics_post_data_rep1_data.csv`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/example_analytics_post_data_rep_data.csv` & `kmds-0.2.9/kmds/examples/example_analytics_post_data_rep_data.csv`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/example_ml_kb_exp_workflow.xml` & `kmds-0.2.9/kmds/examples/example_ml_kb_exp_workflow.xml`

 * *Files 2% similar despite different names*

#### Comparing `kmds-0.2.7/kmds/examples/example_ml_kb_exp_workflow.xml` & `kmds-0.2.9/kmds/examples/example_ml_kb_exp_workflow.xml`

```diff
@@ -209,15 +209,15 @@
     <has_exploratory_observations rdf:resource="#exploratoryobservation2"/>
     <has_exploratory_observations rdf:resource="#exploratoryobservation5"/>
     <has_exploratory_observations rdf:resource="#exploratoryobservation6"/>
     <has_exploratory_observations rdf:resource="#exploratoryobservation1"/>
     <has_exploratory_observations rdf:resource="#exploratoryobservation3"/>
     <has_data_representation_observations rdf:resource="#datarepresentationobservation1"/>
     <has_modeling_choice_observations rdf:resource="#modellingchoiceobservation1"/>
-    <has_model_selection_observations rdf:resource="#modelselectionobservation1"/>
+    <has_model_selection_observations rdf:resource="#modelselectionobservation2"/>
   </owl:NamedIndividual>
   <owl:NamedIndividual rdf:about="#exploratoryobservation4">
     <rdf:type rdf:resource="#ExploratoryObservation"/>
     <finding rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Some Prices are not numbers, these correspond to transactions that are some kind of adjustment - like returns, or,denoting some kind of payment adjustment.</finding>
     <finding_sequence rdf:datatype="http://www.w3.org/2001/XMLSchema#integer">4</finding_sequence>
     <exploratory_observation_type rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Data Quality Observation</exploratory_observation_type>
   </owl:NamedIndividual>
@@ -265,8 +265,14 @@
   </owl:NamedIndividual>
   <owl:NamedIndividual rdf:about="#modelselectionobservation1">
     <rdf:type rdf:resource="#ModelSelectionObservation"/>
     <finding rdf:datatype="http://www.w3.org/2001/XMLSchema#string">For this iteration, PCA was the only modelling approach to explain the variance in dailyproduct sales. This is sufficient to illustrate how a model selection workflow is logged with KMDS.</finding>
     <finding_sequence rdf:datatype="http://www.w3.org/2001/XMLSchema#integer">1</finding_sequence>
     <model_selection_observation_type rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Model Selection Statement</model_selection_observation_type>
   </owl:NamedIndividual>
+  <owl:NamedIndividual rdf:about="#modelselectionobservation2">
+    <rdf:type rdf:resource="#ModelSelectionObservation"/>
+    <finding rdf:datatype="http://www.w3.org/2001/XMLSchema#string">For this iteration, PCA was the only modelling approach to explain the variance in dailyproduct sales. This is sufficient to illustrate how a model selection workflow is logged with KMDS.</finding>
+    <finding_sequence rdf:datatype="http://www.w3.org/2001/XMLSchema#integer">1</finding_sequence>
+    <model_selection_observation_type rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Model Selection Statement</model_selection_observation_type>
+  </owl:NamedIndividual>
 </rdf:RDF>
```

### Comparing `kmds-0.2.7/kmds/examples/incident_event_log_02.csv` & `kmds-0.2.9/kmds/examples/incident_event_log_02.csv`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/online_retail_Q1_2010.parquet` & `kmds-0.2.9/kmds/examples/online_retail_Q1_2010.parquet`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/q2_2016_ticket_resolution_data.csv` & `kmds-0.2.9/kmds/examples/q2_2016_ticket_resolution_data.csv`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/retail_q1_post_EDA.parquet` & `kmds-0.2.9/kmds/examples/retail_q1_post_EDA.parquet`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/retail_q1_post_data_rep_prep.parquet` & `kmds-0.2.9/kmds/examples/retail_q1_post_data_rep_prep.parquet`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/retail_q1_post_mc.parquet` & `kmds-0.2.9/kmds/examples/retail_q1_post_mc.parquet`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/retail_q1_sales_2010_summary.parquet` & `kmds-0.2.9/kmds/examples/retail_q1_sales_2010_summary.parquet`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/test_kb_app_workflow` & `kmds-0.2.9/kmds/examples/test_kb_app_workflow`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/test_kb_app_workflow.xml` & `kmds-0.2.9/kmds/examples/test_kb_app_workflow.xml`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/test_kb_exp_workflow` & `kmds-0.2.9/kmds/examples/test_kb_exp_workflow`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/test_kb_exp_workflow.xml` & `kmds-0.2.9/kmds/examples/test_kb_exp_workflow.xml`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/examples/ticket_resolution_Q2_2016.csv` & `kmds-0.2.9/kmds/examples/ticket_resolution_Q2_2016.csv`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/ontology/kmds_ontology.py` & `kmds-0.2.9/kmds/ontology/kmds_ontology.py`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/ontology/kmds_ontology.xml` & `kmds-0.2.9/kmds/ontology/kmds_ontology.xml`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/pipelines/retail_processing.py` & `kmds-0.2.9/kmds/pipelines/retail_processing.py`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/tagging/tag_types.py` & `kmds-0.2.9/kmds/tagging/tag_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,50 +3,55 @@
 class ExploratoryTags(str, Enum):
     """ Tags to capture the exploratory observation type
 
     Args:
         str (_type_): string type tag
         Enum (_type_): string type tag
     """
+
     RELEVANCE_OBSERVATION = "Relevance Observation" 
     DATA_QUALITY_OBSERVATION = "Data Quality Observation"
 
 class DataRepresentationTags(str, Enum):
     """ Tags to capture the data representation observation type
     Args:
         str (_type_): string type tag
         Enum (_type_): string type tag
     """
+
     FEATURE_ENGG_OBSERVATION = "Feature Engineering Observation"
     DATA_TRANSFORMATION_OBSERVATION = "Data Transformation Observation"
 
 class ModellingChoiceTags(str, Enum):
     """ Tags corresponding to Modelling choice observation type
     Args:
         str (_type_): string type tag
         Enum (_type_): string type tag
     """
+
     MODELLING_CHOICE_OBSERVATION = "Modelling Choice Observation"
     MODELLING_ASSUMPTION_OBSERVATION = "Modelling Assumption Observation"
 
 class ExperimentationTags(str, Enum):
     """ Tags corresponding to experimentation observation type
     Args:
         str (_type_): string type tag
         Enum (_type_): string type tag
     """
+
     HYPOTHESIS_STATEMENT = "Hypothesis Statement"
     EXPERIMENTAL_OBSERVATION = "Experimental Observation"
     EXPERIMENTAL_CONJECTURE = "Experimental Conjecture"
     RESULT_SUMMARY = "Experimental Result Summary"
 
 class ModelSelectionTags(str, Enum):
     """ Tags corresponding to Model Selection observation type
     Args:
         str (_type_): string type tag
         Enum (_type_): string type tag
     """
+    
     MODEL_SELECTION_STATEMENT = "Model Selection Statement"
     MODEL_SELECTION_SETUP_DESCRIPTION = "Model Selection Setup Description"
     MODEL_SELECTION_OBSERVATION = "Model Selection Observation"
     MODEL_SELECTION_RESULT_SUMMARY = "Model Selection Result Summary"
```

### Comparing `kmds-0.2.7/kmds/utils/config_reader.py` & `kmds-0.2.9/kmds/utils/config_reader.py`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/utils/load_utils.py` & `kmds-0.2.9/kmds/utils/load_utils.py`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/kmds/utils/path_utils.py` & `kmds-0.2.9/kmds/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `kmds-0.2.7/PKG-INFO` & `kmds-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmds
-Version: 0.2.7
+Version: 0.2.9
 Summary: This is a package that helps data scientists and data analysts to capture notes while they work through data science tasks. The captured tasks can then be searched and analyzed.
 License: Apache 2.0
 Author: Rajiv Sambasivan
 Author-email: rajiv.sambasivan@r2-ds.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,42 +14,44 @@
 Requires-Dist: Flask (>=3.0.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: owlready2 (>=0.45,<0.46)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Description-Content-Type: text/markdown
 
+[![DOI](https://zenodo.org/badge/753950832.svg)](https://zenodo.org/doi/10.5281/zenodo.10695270)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 <p align="center">
   <img width="460" height="300" src="images/kmds_logo_resized.jpg">
 </p>
 
 ## Knowledge Management for Data Science
 
 ### What is this tool used for?
 
-This tool is used for knowledge management in data science. In software design, conceptual domain models inform lower-level models. In data science work, experiments yield knowledge that informs modeling choices. Data science models are almost always informed by a variety of analysis experiments. Experimentation and organization of knowledge artifacts supporting modeling decisions a requirement for reproducible data science models and improving model quality and performance.
+This tool is used for knowledge management in data science. In software design, conceptual domain models inform lower-level models. In data science work, experiments yield knowledge that informs modeling choices. Data science models are almost always informed by a variety of analysis experiments. Experimentation and organization of knowledge artifacts supporting modeling decisions is a requirement for reproducible data science models and improving model quality and performance.
 
 Please see [knowledge application development context](/feature_documentation/knowledge_management_in_DS.md ) for a description of a typical knowledge application development setting.
 
 ### Why do you need this tool?
 
-The above narrative suggests that ability to retrieve knowledge about experiments and historical models in an adhoc manner is critical in data science. It is. It is also grossly underserved. Knowledge management tools for domain specific models exist, knowledge management tools for dev-ops and ML-Ops exist, but tools for analytics and model development are siloed. Information gets fragmented over time. So analysts and data scientists often have to go to experiment tools, data catalogs or ML-Ops tools to fetch information they need to develop a model. In a subsequent iteration of this model, the contextual information that informed the development of this model if often lost and the development team, possibly with new team members, have the task of reconstructing this contextual information again. This library is a step in fixing this problem. The central idea is to organize tasks in terms of a sequence of steps that are pretty standard in data analysis work and capture knowledge in context while these tasks are performed.
+The above narrative suggests that ability to retrieve knowledge about experiments and historical models in an adhoc manner is critical in data science. It is. It is also grossly underserved. Knowledge management tools for domain specific models exist, knowledge management tools for dev-ops and ML-Ops exist, but tools for analytics and model development are siloed. Information gets fragmented over time. So analysts and data scientists often have to go to experiment tools, data catalogs or ML-Ops tools to fetch information they need to develop a model. In a subsequent iteration of this model, the contextual information that informed the development of this model is often lost, and the development team, possibly with new team members, have the task of reconstructing this contextual information again. This library is a step in fixing this problem. The central idea is to organize tasks in terms of a sequence of steps that are pretty standard in data analysis work and capture knowledge in context while these tasks are performed.
 
 ### How is it related to process guidelines and vocabularies for machine learning?
 Initiatives such as [CRISP DM](https://www.datascience-pm.com/crisp-dm-2/) provide guidelines and processes for developing data science projects. Projects such as [Open ML](https://openml.github.io/openml-python/main/index.html) provide semantic vocabulary standardization for machine learning tasks. These are excellent tools. However, the guidelines they provide are task focussed. The gap between a conceptual idea and the final, or, even candidate data science tasks for a project is filled with many assumptions and experimental evaluations. The information in these assumptions and experimental evaluations is what this tool aims to capture. There is also an ordering to these assumptions and experimental evaluations. This is also what this tool aims to capture.
 
 ### Who would use this tool?
 
 This tool is for data scientists and data analysts.
 
 ### How do you use this tool?
 
 1. You install this library along with the other python dependecies you need for your analysis task
 2. Review the [basic recipe](examples_of_use/workflow_recipe.md) for capturing your observations.
-3. Review [the templates section](examples_of_use/workflow_recipe.md) to find illustrative examples of the process to use this tool to capture knowledge facts in your data science workflows. For analytics projects, review the analytics template. For machine learning projects, review the machine learning template.
+3. Review [the templates section](examples_of_use/workflow_recipe.md) to find the example relevant to you. For analytics projects, review the analytics template. For machine learning projects, review the machine learning template.
 4. Start using the tool in your projects using the information from your review of the above two steps.
 
 ### Licensing and Feature Questions
 
 1. The tool is open source with an [apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0.txt)
 2. If you are interested in the following features, please set up a [meeting](https://calendly.com/rajiv-sambasivan/help-with-kmds-feature) with me:
    1. Help with a data analysis task for your use case
```

