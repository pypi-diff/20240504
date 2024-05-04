# Comparing `tmp/sapiopycommons-31.2.0.23.12.3.tar.gz` & `tmp/sapiopycommons-31.3.0.23.12.3.tar.gz`

## Comparing `sapiopycommons-31.2.0.23.12.3.tar` & `sapiopycommons-31.3.0.23.12.3.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/Molecules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/__init__.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/__init__.py
--rw-r--r--   0        0        0    54417 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/__init__.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_bridge.py
--rw-r--r--   0        0        0    23142 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/aliases.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/custom_report_util.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/exceptions.py
--rw-r--r--   0        0        0    29150 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/popup_util.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/time_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/__init__.py
--rw-r--r--   0        0        0    34338 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/__init__.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/__init__.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/LICENSE
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/pyproject.toml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/Molecules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/datatype/__init__.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/eln/__init__.py
+-rw-r--r--   0        0        0    57231 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/__init__.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/complex_data_loader.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/file_bridge.py
+-rw-r--r--   0        0        0    23383 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/file_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/__init__.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/aliases.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/custom_report_util.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/exceptions.py
+-rw-r--r--   0        0        0    29112 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/popup_util.py
+-rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/storage_util.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/time_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/processtracking/__init__.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/processtracking/endpoints.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/recordmodel/__init__.py
+-rw-r--r--   0        0        0    35178 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/__init__.py
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py
+-rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/webhook/__init__.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/LICENSE
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/pyproject.toml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sapiopycommons-31.3.0.23.12.3/PKG-INFO
```

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/Molecules.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/chem/Molecules.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,20 +63,26 @@
     """Entry options for each step in this experiment. Only cached for each individual step when they are first accessed.
     The cache is updated whenever the entry options for a step are changed by this handler."""
 
     # Constants
     # TODO: sapiopylib is currently storing the status of entries as strings when first queried, requiring us to compare
     #  against the value of the enums instead of the enums themselves. The ".value"s can be removed once sapiopylib is
     #  fixed.
-    __COMPLETE_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value]
+    __ENTRY_COMPLETE_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value]
     """The set of statuses that an ELN entry could have and be considered completed/submitted."""
-    __LOCKED_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value,
-                         ExperimentEntryStatus.Disabled.value, ExperimentEntryStatus.LockedAwaitingApproval.value,
-                         ExperimentEntryStatus.LockedRejected.value]
+    __ENTRY_LOCKED_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value,
+                               ExperimentEntryStatus.Disabled.value, ExperimentEntryStatus.LockedAwaitingApproval.value,
+                               ExperimentEntryStatus.LockedRejected.value]
     """The set of statuses that an ELN entry could have and be considered locked."""
+    __EXPERIMENT_COMPLETE_STATUSES = [ElnExperimentStatus.Completed, ElnExperimentStatus.CompletedApproved]
+    """The set of statuses that an ELN experiment could have and be considered completed."""
+    __EXPERIMENT_LOCKED_STATUSES = [ElnExperimentStatus.Completed, ElnExperimentStatus.CompletedApproved,
+                                    ElnExperimentStatus.LockedRejected, ElnExperimentStatus.LockedAwaitingApproval,
+                                    ElnExperimentStatus.Canceled]
+    """The set of statuses that an ELN experiment could have and be considered locked."""
 
     def __init__(self, context: SapioWebhookContext, experiment: ElnExperiment | None = None):
         """
         Initialization will throw an exception if there is no ELN Experiment in the provided context and no experiment
         is provided.
 
         :param context: The current webhook context.
@@ -346,14 +352,61 @@
             (e.g. a Dict). If an option key already exists and is provided in the mapping, overwrites the existing value
             for that key.
         """
         options: dict[str, str] = self.get_experiment_options()
         options.update(mapping)
         self.update_experiment(experiment_option_map=options)
 
+    def experiment_is_complete(self) -> bool:
+        """
+        Determine if the experiment has been completed.
+
+        :return: True if the experiment's status is Completed or CompletedApproved. False otherwise.
+        """
+        return self.__eln_exp.notebook_experiment_status in self.__EXPERIMENT_COMPLETE_STATUSES
+
+    def experiment_is_canceled(self) -> bool:
+        """
+        Determine if the experiment has been canceled.
+
+        :return: True if the experiment's status is Canceled. False otherwise.
+        """
+        return self.__eln_exp.notebook_experiment_status == ElnExperimentStatus.Canceled
+
+    def experiment_is_locked(self) -> bool:
+        """
+        Determine if the experiment has been locked in any way.
+
+        :return: True if the experiment's status is Completed, CompletedApproved, Canceled, LockedAwaitingApproval,
+            or LockedRejected. False otherwise.
+        """
+        return self.__eln_exp.notebook_experiment_status in self.__EXPERIMENT_LOCKED_STATUSES
+
+    def complete_experiment(self) -> None:
+        """
+        Set the experiment's status to Completed. Makes a webservice call to update the experiment. Checks if the
+        experiment is already completed, and does nothing if so.
+        """
+        if not self.experiment_is_complete():
+            self.__protocol.complete_protocol()
+            self.__eln_exp.notebook_experiment_status = ElnExperimentStatus.Completed
+
+    def cancel_experiment(self) -> None:
+        """
+        Set the experiment's status to Canceled. Makes a webservice call to update the experiment. Checks if the
+        experiment is already canceled, and does nothing if so.
+
+        NOTE: This will not run the usual logic around canceling an experiment that you'd see if canceling the
+        experiment using the "Cancel Experiment" toolbar button, such as moving in process samples back to the queue,
+        as those changes are tied to the button instead of being on the experiment status change.
+        """
+        if not self.experiment_is_canceled():
+            self.__protocol.cancel_protocol()
+            self.__eln_exp.notebook_experiment_status = ElnExperimentStatus.Canceled
+
     def step_exists(self, step_name: str) -> bool:
         """
         Determine if a step by the given name exists in the experiment.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
 
@@ -863,15 +916,15 @@
 
         :param step:
             The step to complete.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         step = self.__to_eln_step(step)
-        if step.eln_entry.entry_status not in self.__COMPLETE_STATUSES:
+        if step.eln_entry.entry_status not in self.__ENTRY_COMPLETE_STATUSES:
             step.complete_step()
             # TODO: sapiopylib is currently storing the status of entries as strings when first queried. For the sake of not
             #  breaking comparisons to enums that expect this behavior, also setting the status to the enum's string.
             #  The ".value" can be removed once sapiopylib is fixed.
             step.eln_entry.entry_status = ExperimentEntryStatus.Completed.value
 
     def unlock_step(self, step: Step) -> None:
@@ -884,15 +937,15 @@
 
         :param step:
             The step to unlock.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         step = self.__to_eln_step(step)
-        if step.eln_entry.entry_status in self.__LOCKED_STATUSES:
+        if step.eln_entry.entry_status in self.__ENTRY_LOCKED_STATUSES:
             step.unlock_step()
             # TODO: sapiopylib is currently storing the status of entries as strings when first queried. For the sake of not
             #  breaking comparisons to enums that expect this behavior, also setting the status to the enum's string.
             #  The ".value" can be removed once sapiopylib is fixed.
             step.eln_entry.entry_status = ExperimentEntryStatus.UnlockedChangesRequired.value
 
     def step_is_submitted(self, step: Step) -> bool:
@@ -904,15 +957,15 @@
 
         :param step:
             The step to check.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :return: True if the step's status is Completed or CompletedApproved. False otherwise.
         """
-        return self.__to_eln_step(step).eln_entry.entry_status in self.__COMPLETE_STATUSES
+        return self.__to_eln_step(step).eln_entry.entry_status in self.__ENTRY_COMPLETE_STATUSES
 
     def step_is_locked(self, step: Step) -> bool:
         """
         Determine if the input step has been locked in any way.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
@@ -920,15 +973,15 @@
         :param step:
             The step to check.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :return: True if the step's status is Completed, CompletedApproved, Disabled, LockedAwaitingApproval,
             or LockedRejected. False otherwise.
         """
-        return self.__to_eln_step(step).eln_entry.entry_status in self.__LOCKED_STATUSES
+        return self.__to_eln_step(step).eln_entry.entry_status in self.__ENTRY_LOCKED_STATUSES
 
     def __to_eln_step(self, step: Step) -> ElnEntryStep:
         """
         Convert a variable that could be either a string or an ElnEntryStep to just an ElnEntryStep.
         This will query and cache the steps for the experiment if the input step is a name and the steps have not been
         cached before.
```

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_bridge.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/file_bridge.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_util.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/files/file_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,19 +346,23 @@
                 # Empty cells get added to the list as None.
                 if value == "nan":
                     value = None
                 row.update({header: value})
 
         # Warn about improper headers. Confirm that the header contains each of the header column names that we want.
         if required_headers is not None:
+            # FR-46702: Report all missing headers instead of only the first missing header.
+            missing_headers: list[str] = []
             for required in required_headers:
                 if required not in witnessed_headers:
-                    at_row = " at row " + str(header_row_index + 1) if header_row_index is not None else ""
-                    raise SapioUserErrorException(f"Incorrect file headers or incorrectly formatted table. Header \""
-                                                  f"{required}\" not found{at_row}.")
+                    missing_headers.append("\"" + required + "\"")
+            if missing_headers:
+                at_row = " at row " + str(header_row_index + 1) if header_row_index is not None else ""
+                raise SapioUserErrorException(f"Incorrect file headers or incorrectly formatted table. Header(s) "
+                                              f"{', '.join(missing_headers)} not found{at_row}.")
 
         return rows
 
     @staticmethod
     def csv_to_xlsx(file_data: bytes | str) -> bytes:
         """
         Convert a CSV file into an XLSX file.
```

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/custom_report_util.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/custom_report_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/exceptions.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/popup_util.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/popup_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-from typing import Any
-
 from sapiopylib.rest.DataMgmtService import DataMgmtServer
 from sapiopylib.rest.pojo.datatype.DataType import DataTypeDefinition
 from sapiopylib.rest.pojo.datatype.FieldDefinition import VeloxStringFieldDefinition, AbstractVeloxFieldDefinition, \
     VeloxIntegerFieldDefinition, VeloxDoubleFieldDefinition
 from sapiopylib.rest.pojo.webhook.ClientCallbackRequest import FormEntryDialogRequest, OptionDialogRequest, \
     TableEntryDialogRequest, ListDialogRequest, DataRecordSelectionRequest
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
 from sapiopylib.rest.pojo.webhook.WebhookResult import SapioWebhookResult
 from sapiopylib.rest.utils.FormBuilder import FormBuilder
 
-from sapiopycommons.general.aliases import SapioRecord, AliasUtil
+from sapiopycommons.general.aliases import SapioRecord, AliasUtil, FieldMap
 from sapiopycommons.general.exceptions import SapioException
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 # FR-46097 - Greatly expand the options that PopupUtil provides. (Originally just had two OptionDialogRequest
 # and one FormEntryDialogRequest methods.)
 # CR-46332 - For any functions that use temporary data types, set the data type name, display name, and plural display
 # name in the form builder.
 class PopupUtil:
     """
     Methods for creating boilerplate SapioWebhookResults with client callback requests to create popup dialogs.
     """
     @staticmethod
-    def form_popup(title: str, msg: str, fields: list[AbstractVeloxFieldDefinition], values: dict[str, Any] = None,
+    def form_popup(title: str, msg: str, fields: list[AbstractVeloxFieldDefinition], values: FieldMap = None,
                    column_positions: dict[str, tuple[int, int]] = None, data_type: str = "Default",
                    *, display_name: str | None = None, plural_display_name: str | None = None,
                    request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a basic form entry dialog.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
@@ -222,15 +220,15 @@
             default_value = min_value
         double_field = VeloxDoubleFieldDefinition(data_type, field_name, field_name, default_value=default_value,
                                                   min_value=min_value, max_value=max_value, editable=editable, **kwargs)
         return PopupUtil.form_popup(title, msg, [double_field], data_type=data_type, display_name=display_name,
                                     plural_display_name=plural_display_name, request_context=request_context)
 
     @staticmethod
-    def table_popup(title: str, msg: str, fields: list[AbstractVeloxFieldDefinition], values: list[dict[str, Any]],
+    def table_popup(title: str, msg: str, fields: list[AbstractVeloxFieldDefinition], values: list[FieldMap],
                     *, data_type: str = "Default", display_name: str | None = None,
                     plural_display_name: str | None = None, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a basic table entry dialog.
 
         The calling webhook must catch the TableEntryDialogResult that the client will send back.
 
@@ -281,15 +279,15 @@
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         data_types: set[str] = {x.data_type_name for x in records}
         if len(data_types) > 1:
             raise SapioException("Multiple data type names encountered in records list for record table popup.")
         data_type: str = data_types.pop()
         # Get the field maps from the records.
-        field_map_list: list[dict[str, Any]] = AliasUtil.to_field_map_lists(records)
+        field_map_list: list[FieldMap] = AliasUtil.to_field_map_lists(records)
         # Get the field definitions of the data type.
         type_man = DataMgmtServer.get_data_type_manager(context.user)
         type_def: DataTypeDefinition = type_man.get_data_type_definition(data_type)
         field_defs: dict[str, AbstractVeloxFieldDefinition] = {x.data_field_name: x for x in
                                                                type_man.get_field_definition_list(data_type)}
 
         # Build the form using only those fields that are desired.
@@ -331,15 +329,15 @@
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         data_types: set[str] = {x.data_type_name for x in records}
         if len(data_types) > 1:
             raise SapioException("Multiple data type names encountered in records list for record table popup.")
         data_type: str = data_types.pop()
         # Get the field maps from the records.
-        field_map_list: list[dict[str, Any]] = AliasUtil.to_field_map_lists(records)
+        field_map_list: list[FieldMap] = AliasUtil.to_field_map_lists(records)
         # Get the field definitions of the data type.
         type_man = DataMgmtServer.get_data_type_manager(context.user)
         type_def: DataTypeDefinition = type_man.get_data_type_definition(data_type)
         field_defs: dict[str, AbstractVeloxFieldDefinition] = {x.data_field_name: x for x in
                                                                type_man.get_field_definition_list(data_type)}
 
         # Build the form using only those fields that are desired.
```

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/time_util.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/general/time_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
 from sapiopylib.rest.utils.recordmodel.PyRecordModel import PyRecordModel
 from sapiopylib.rest.utils.recordmodel.RecordModelManager import RecordModelManager, RecordModelInstanceManager, \
     RecordModelRelationshipManager
 from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedType
 from sapiopylib.rest.utils.recordmodel.RelationshipPath import RelationshipPath, RelationshipPathDir
 
-from sapiopycommons.general.aliases import RecordModel, SapioRecord
+from sapiopycommons.general.aliases import RecordModel, SapioRecord, FieldMap
 from sapiopycommons.general.custom_report_util import CustomReportUtil
 from sapiopycommons.general.exceptions import SapioException
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class RecordHandler:
     """
@@ -189,15 +189,15 @@
 
         :param wrapper_type: The record model wrapper to use.
         :param num: The number of models to create.
         :return: The newly added record models.
         """
         return self.inst_man.add_new_records_of_type(num, wrapper_type)
 
-    def add_models_with_data(self, wrapper_type: type[WrappedType], fields: list[dict[str, Any]]) -> list[WrappedType]:
+    def add_models_with_data(self, wrapper_type: type[WrappedType], fields: list[FieldMap]) -> list[WrappedType]:
         """
         Shorthand for using the instance manager to add new models of the given type, and then initializing all those
         models with the given fields.
 
         :param wrapper_type: The record model wrapper to use.
         :param fields: A list of field maps to initialize the record models with.
         :return: The newly added record models with the provided fields set. The records will be in the same order as
@@ -218,15 +218,15 @@
         :param wrapper_type: The record model wrapper to use.
         :param num: The number of new records to create.
         :return: The newly created record models.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
         return self.wrap_models(self.dr_man.add_data_records(dt, num), wrapper_type)
 
-    def create_models_with_data(self, wrapper_type: type[WrappedType], fields: list[dict[str, Any]]) \
+    def create_models_with_data(self, wrapper_type: type[WrappedType], fields: list[FieldMap]) \
             -> list[WrappedType]:
         """
         Shorthand for creating new records via the data record manager with field data to initialize the records with
         and then returning them as wrapped record models. Useful in cases where your record model needs to have a valid
         record ID.
 
         Makes a webservice call to create the data records.
@@ -235,15 +235,15 @@
         :param fields: The field map list to initialize the new data records with.
         :return: The newly created record models.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
         return self.wrap_models(self.dr_man.add_data_records_with_data(dt, fields), wrapper_type)
 
     def find_or_create_model(self, wrapper_type: type[WrappedType], primary_identifier: str, id_value: Any,
-                             secondary_identifiers: dict[str, Any] | None = None) -> WrappedType:
+                             secondary_identifiers: FieldMap | None = None) -> WrappedType:
         """
         Find a unique record that matches the given field values. If no such records exist, create one with the
         identifying fields set to the desired values. If more than one record with the identifying values exists,
         throws an exception.
 
         The record is searched for using the primary identifier field name and value. If multiple records are returned
         by the query on this primary identifier, then the secondary identifiers are used to filter the results.
@@ -288,45 +288,47 @@
         # If none of the results matched the identifiers, create a new record with all identifiers set.
         # Put the primary identifier and value into the secondary identifiers list and use that as the fields map
         # for this new record.
         secondary_identifiers.update({primary_identifier: id_value})
         return self.create_models_with_data(wrapper_type, [secondary_identifiers])[0]
 
     @staticmethod
-    def map_to_parent(models: Iterable[RecordModel], parent_type: type[WrappedType]) -> dict:
+    def map_to_parent(models: Iterable[RecordModel], parent_type: type[WrappedType]) -> dict[RecordModel, WrappedType]:
         """
         Map a list of record models to a single parent of a given type. The parents must already be loaded.
 
         :param models: A list of record models.
         :param parent_type: The record model wrapper of the parent.
         :return: A dict[ModelType, ParentType]. If an input model doesn't have a parent of the given parent type, then
             it will map to None.
         """
         return_dict: dict[RecordModel, WrappedType] = {}
         for model in models:
             return_dict[model] = model.get_parent_of_type(parent_type)
         return return_dict
 
     @staticmethod
-    def map_to_parents(models: Iterable[RecordModel], parent_type: type[WrappedType]) -> dict:
+    def map_to_parents(models: Iterable[RecordModel], parent_type: type[WrappedType]) \
+            -> dict[RecordModel, list[WrappedType]]:
         """
         Map a list of record models to a list parents of a given type. The parents must already be loaded.
 
         :param models: A list of record models.
         :param parent_type: The record model wrapper of the parents.
         :return: A dict[ModelType, list[ParentType]]. If an input model doesn't have a parent of the given parent type,
             then it will map to an empty list.
         """
         return_dict: dict[RecordModel, list[WrappedType]] = {}
         for model in models:
             return_dict[model] = model.get_parents_of_type(parent_type)
         return return_dict
 
     @staticmethod
-    def map_by_parents(models: Iterable[RecordModel], parent_type: type[WrappedType]) -> dict:
+    def map_by_parents(models: Iterable[RecordModel], parent_type: type[WrappedType]) \
+            -> dict[WrappedType, list[RecordModel]]:
         """
         Take a list of record models and map them by their parents. Essentially an inversion of map_to_parents. Input
         models that share a parent will end up in the same list. The parents must already be loaded.
 
         :param models: A list of record models.
         :param parent_type: The record model wrapper of the parents.
         :return: A dict[ParentType, list[ModelType]]. If an input model doesn't have a parent of the given parent type,
@@ -336,52 +338,54 @@
         by_parents: dict[WrappedType, list[RecordModel]] = {}
         for record, parents in to_parents.items():
             for parent in parents:
                 by_parents.setdefault(parent, []).append(record)
         return by_parents
 
     @staticmethod
-    def map_to_child(models: Iterable[RecordModel], child_type: type[WrappedType]) -> dict:
+    def map_to_child(models: Iterable[RecordModel], child_type: type[WrappedType]) -> dict[RecordModel, WrappedType]:
         """
         Map a list of record models to a single child of a given type. The children must already be loaded.
 
         :param models: A list of record models.
         :param child_type: The record model wrapper of the child.
         :return: A dict[ModelType, ChildType]. If an input model doesn't have a child of the given child type, then
             it will map to None.
         """
         return_dict: dict[RecordModel, WrappedType] = {}
         for model in models:
             return_dict[model] = model.get_child_of_type(child_type)
         return return_dict
 
     @staticmethod
-    def map_to_children(models: Iterable[RecordModel], child_type: type[WrappedType]) -> dict:
+    def map_to_children(models: Iterable[RecordModel], child_type: type[WrappedType]) \
+            -> dict[RecordModel, list[WrappedType]]:
         """
         Map a list of record models to a list children of a given type. The children must already be loaded.
 
         :param models: A list of record models.
         :param child_type: The record model wrapper of the children.
         :return: A dict[ModelType, list[ChildType]]. If an input model doesn't have children of the given child type,
             then it will map to an empty list.
         """
         return_dict: dict[RecordModel, list[WrappedType]] = {}
         for model in models:
             return_dict[model] = model.get_children_of_type(child_type)
         return return_dict
 
     @staticmethod
-    def map_by_children(models: Iterable[RecordModel], child_type: type[WrappedType]) -> dict:
+    def map_by_children(models: Iterable[RecordModel], child_type: type[WrappedType]) \
+            -> dict[WrappedType, list[RecordModel]]:
         """
         Take a list of record models and map them by their children. Essentially an inversion of map_to_children. Input
         models that share a child will end up in the same list. The children must already be loaded.
 
         :param models: A list of record models.
         :param child_type: The record model wrapper of the children.
-        :return: A dict[ParentType, list[ModelType]]. If an input model doesn't have children of the given child type,
+        :return: A dict[ChildType, list[ModelType]]. If an input model doesn't have children of the given child type,
             then it will not be in the resulting dictionary.
         """
         to_children: dict[RecordModel, list[WrappedType]] = RecordHandler.map_to_children(models, child_type)
         by_children: dict[WrappedType, list[RecordModel]] = {}
         for record, children in to_children.items():
             for child in children:
                 by_children.setdefault(child, []).append(record)
@@ -471,17 +475,32 @@
         """
         newest: SapioRecord | None = None
         for record in records:
             if newest is None or record.record_id > newest.record_id:
                 newest = record
         return newest
 
+    # FR-46696: Add a function for getting the oldest record in a list, just like we have one for the newest record.
     @staticmethod
-    def values_to_field_maps(field_name: str, values: Iterable[Any], existing_fields: list[dict[str, Any]] | None = None) \
-            -> list[dict[str, Any]]:
+    def get_oldest_record(records: Iterable[SapioRecord]) -> SapioRecord:
+        """
+        Get the oldest record from a list of records.
+
+        :param records: The list of records.
+        :return: The input record with the lowest record ID. None if the input list is empty.
+        """
+        oldest: SapioRecord | None = None
+        for record in records:
+            if oldest is None or record.record_id < oldest.record_id:
+                oldest = record
+        return oldest
+
+    @staticmethod
+    def values_to_field_maps(field_name: str, values: Iterable[Any], existing_fields: list[FieldMap] | None = None) \
+            -> list[FieldMap]:
         """
         Add a list of values for a specific field to a list of dictionaries pairing each value to that field name.
 
         :param field_name: The name of the field that the values are from.
         :param values: A list of field values.
         :param existing_fields: An optional existing fields map list to add the new values to. Values are added in the
           list in the same order that they appear. If no existing fields are provided, returns a new fields map list.
```

### Comparing `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py` & `sapiopycommons-31.3.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/LICENSE` & `sapiopycommons-31.3.0.23.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/README.md` & `sapiopycommons-31.3.0.23.12.3/README.md`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.2.0.23.12.3/pyproject.toml` & `sapiopycommons-31.3.0.23.12.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopycommons"
-version='31.2.0.23.12.3'
+version='31.3.0.23.12.3'
 authors = [
     { name="Jonathan Steck", email="jsteck@sapiosciences.com" },
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Python API Utilities Package"
 license = "MPL-2.0"
 readme = "README.md"
```

### Comparing `sapiopycommons-31.2.0.23.12.3/PKG-INFO` & `sapiopycommons-31.3.0.23.12.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopycommons
-Version: 31.2.0.23.12.3
+Version: 31.3.0.23.12.3
 Summary: Official Sapio Python API Utilities Package
 Project-URL: Homepage, https://github.com/sapiosciences
 Author-email: Jonathan Steck <jsteck@sapiosciences.com>, Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: sapiopycommons Version: 31.2.0.23.12.3 Summary:
+Metadata-Version: 2.3 Name: sapiopycommons Version: 31.3.0.23.12.3 Summary:
 Official Sapio Python API Utilities Package Project-URL: Homepage, https://
 github.com/sapiosciences Author-email: Jonathan Steck
 sapiosciences.com>, Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
```

