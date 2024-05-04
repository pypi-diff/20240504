# Comparing `tmp/sapiopylib-2024.5.3rc190.tar.gz` & `tmp/sapiopylib-2024.5.4a191.tar.gz`

## Comparing `sapiopylib-2024.5.3rc190.tar` & `sapiopylib-2024.5.4a191.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0    15523 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/ClientCallbackService.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    50807 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataService.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    24628 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/MessengerService.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/ReportManager.py
--rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/Message.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/acl.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    29992 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/field_set.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/protocol_template.py
--rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    26690 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/autopaging.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recorddatasinks.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    28845 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    46989 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/ancestry.py
--rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/properties.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/src/sapiopylib/utils/string.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/CR-52168_test.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/EmailAttachmentDataTest.py
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51536_test.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51549_test.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51551_test.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51635_test.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51821_test.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51846_test.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51847_test.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-51849_test.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-52100_test.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-52133_test.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/FR-52251_test.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/PR-51537_test.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/PR-51547.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/PR-51842_test.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/PR-51853_test.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/PR-51856_test.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/PR-51964_test.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/PR-52136_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/__init__.py
--rw-r--r--   0        0        0  2028234 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/data_type_models.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/resources/NAC28735.fa
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/tests/resources/fr-51846.ssg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/LICENSE
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/pyproject.toml
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 sapiopylib-2024.5.3rc190/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0    15523 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/ClientCallbackService.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    50807 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataService.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    24628 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/MessengerService.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/ReportManager.py
+-rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/Message.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/acl.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
+-rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    29992 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/field_set.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/protocol_template.py
+-rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    26690 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/autopaging.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recorddatasinks.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    28845 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46989 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/ancestry.py
+-rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/properties.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/src/sapiopylib/utils/string.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/CR-52168_test.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/EmailAttachmentDataTest.py
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51536_test.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51549_test.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51551_test.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51635_test.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51821_test.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51846_test.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51847_test.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-51849_test.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-52100_test.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-52133_test.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/FR-52251_test.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/PR-51537_test.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/PR-51547.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/PR-51842_test.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/PR-51853_test.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/PR-51856_test.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/PR-51964_test.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/PR-52136_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/__init__.py
+-rw-r--r--   0        0        0  2028234 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/data_type_models.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/resources/NAC28735.fa
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/tests/resources/fr-51846.ssg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/LICENSE
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/README.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/pyproject.toml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.5.4a191/PKG-INFO
```

### Comparing `sapiopylib-2024.5.3rc190/INSTALL.md` & `sapiopylib-2024.5.4a191/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/ClientCallbackService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/ClientCallbackService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/MessengerService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/MessengerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/ReportManager.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/ReportManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/User.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/Message.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/Message.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/acl.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/acl.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/field_set.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/field_set.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/eln/protocol_template.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/eln/protocol_template.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/autopaging.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/autopaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recorddatasinks.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recorddatasinks.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/ancestry.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/ancestry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/rest/utils/recordmodel/properties.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/rest/utils/recordmodel/properties.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/src/sapiopylib/utils/string.py` & `sapiopylib-2024.5.4a191/src/sapiopylib/utils/string.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/CR-52168_test.py` & `sapiopylib-2024.5.4a191/tests/CR-52168_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/EmailAttachmentDataTest.py` & `sapiopylib-2024.5.4a191/tests/EmailAttachmentDataTest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51536_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51536_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51549_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51549_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51551_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51551_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51635_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51635_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51821_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51821_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51846_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51846_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51847_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51847_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-51849_test.py` & `sapiopylib-2024.5.4a191/tests/FR-51849_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-52100_test.py` & `sapiopylib-2024.5.4a191/tests/FR-52100_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-52133_test.py` & `sapiopylib-2024.5.4a191/tests/FR-52133_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/FR-52251_test.py` & `sapiopylib-2024.5.4a191/tests/FR-52251_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/PR-51537_test.py` & `sapiopylib-2024.5.4a191/tests/PR-51537_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/PR-51547.py` & `sapiopylib-2024.5.4a191/tests/PR-51547.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/PR-51842_test.py` & `sapiopylib-2024.5.4a191/tests/PR-51842_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/PR-51853_test.py` & `sapiopylib-2024.5.4a191/tests/PR-51853_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/PR-51856_test.py` & `sapiopylib-2024.5.4a191/tests/PR-51856_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/PR-51964_test.py` & `sapiopylib-2024.5.4a191/tests/PR-51964_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/PR-52136_test.py` & `sapiopylib-2024.5.4a191/tests/PR-52136_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/data_type_models.py` & `sapiopylib-2024.5.4a191/tests/data_type_models.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/resources/NAC28735.fa` & `sapiopylib-2024.5.4a191/tests/resources/NAC28735.fa`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/tests/resources/fr-51846.ssg` & `sapiopylib-2024.5.4a191/tests/resources/fr-51846.ssg`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/LICENSE` & `sapiopylib-2024.5.4a191/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/README.md` & `sapiopylib-2024.5.4a191/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.5.3rc190/pyproject.toml` & `sapiopylib-2024.5.4a191/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2024.05.03rc190'
+version='2024.05.04a191'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sapiopylib-2024.5.3rc190/PKG-INFO` & `sapiopylib-2024.5.4a191/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopylib
-Version: 2024.5.3rc190
+Version: 2024.5.4a191
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: sapiopylib Version: 2024.5.3rc190 Summary: Official
+Metadata-Version: 2.3 Name: sapiopylib Version: 2024.5.4a191 Summary: Official
 Sapio Informatics Platform Python API Project-URL: Homepage, https://
 github.com/sapiosciences Project-URL: Bug Tracker, https://github.com/
 sapiosciences/sapio-py-tutorials/issues Author-email: Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
```

