# Comparing `tmp/sapiopylib-2023.6.6.140.tar.gz` & `tmp/sapiopylib-2023.6.7.141.tar.gz`

## Comparing `sapiopylib-2023.6.6.140.tar` & `sapiopylib-2023.6.7.141.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    17781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/LICENSE
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/pyproject.toml
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 sapiopylib-2023.6.6.140/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    18143 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25176 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/LICENSE
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/pyproject.toml
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/PKG-INFO
```

### Comparing `sapiopylib-2023.6.6.140/INSTALL.md` & `sapiopylib-2023.6.7.141/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/ELNService.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,22 @@
         """
         sub_path = '/eln/notebookexperiment/'
         response = self.user.post(sub_path, payload=pojo.to_json())
         self.user.raise_for_status(response)
         json_dict = response.json()
         return ELNExperimentParser.parse_eln_experiment(json_dict)
 
+    def delete_notebook_experiment(self, notebook_experiment_id: int) -> None:
+        """
+        Delete a notebook experiment when providing a notebook experiment ID.
+        """
+        subpath = self.user.build_url(['eln', 'experiment', str(notebook_experiment_id)])
+        response = self.user.delete(subpath)
+        self.user.raise_for_status(response)
+
     def get_template_experiment_list(self, query: TemplateExperimentQueryPojo) -> List[ElnTemplate]:
         """
         Get a list of TemplateExperimentPojo objects using the provided criteria object to search
         the templates in the app.
         :return: List of templates matching the provided criteria in the system.
         """
         sub_path = "/eln/templateexperiment/"
```

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/User.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(self):
         self.chart_guid = None
         self.dashboard_guid = None
         self.display_name = None
         self.description = None
         self.series_list = None
         self.main_data_type_name = None
-        self.grouping_type = None
+        self.grouping_type = ChartGroupingType.NO_GROUPING
         self.grouping_type_data_type_name = None
         self.grouping_type_data_field_name = None
         self.created_by = None
         self.date_created = None
 
     @abstractmethod
     def get_chart_type(self) -> ChartType:
```

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import List, Optional, Dict, Tuple
 
 from sapiopylib.rest.DataMgmtService import DataMgmtServer
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 from sapiopylib.rest.pojo.chartdata.DashboardDefinition import BarLineChartDefinition, DashboardDefinition, \
-    XyChartDefinition, HeatMapChartDefinition
+    XyChartDefinition, HeatMapChartDefinition, GanttChartDefinition
 from sapiopylib.rest.pojo.chartdata.DashboardEnums import ChartGroupingType, \
     ChartOperationType, DashboardScope, PointShapeType, LineStyleType
-from sapiopylib.rest.pojo.chartdata.DashboardSeries import BarChartSeries, XyChartSeries, HeatMapChartSeries
+from sapiopylib.rest.pojo.chartdata.DashboardSeries import BarChartSeries, XyChartSeries, HeatMapChartSeries, \
+    GanttChartSeries
 from sapiopylib.rest.pojo.eln.ExperimentEntry import ExperimentEntry
 from sapiopylib.rest.pojo.eln.ExperimentEntryCriteria import ElnEntryCriteria, ELNFormEntryUpdateCriteria, \
     ElnPluginEntryUpdateCriteria, ElnDashboardEntryUpdateCriteria
 from sapiopylib.rest.pojo.eln.SapioELNEnums import ElnEntryType, ElnBaseDataType
 from sapiopylib.rest.utils.Protocols import ElnExperimentProtocol, ElnEntryStep
 from sapiopylib.rest.utils.plates.MultiLayerPlating import MultiLayerPlateConfig, MultiLayerPlateLayer
 from sapiopylib.rest.utils.plates.MultiLayerPlatingUtils import MultiLayerPlatingManager
@@ -39,22 +40,21 @@
 
 class ELNStepFactory:
     """
     Factory that provides simple functions to create a new ELN step under an ELN protocol.
     """
 
     @staticmethod
-    def _create_dashboard_step_from_chart(chart, data_source_step, data_type_name, protocol, step_name) -> \
+    def _create_dashboard_step_from_chart(chart, data_source_step, protocol, step_name) -> \
             Tuple[DashboardDefinition, ElnEntryStep]:
         dashboard: DashboardDefinition = DashboardDefinition()
         dashboard.chart_definition_list = [chart]
         dashboard.dashboard_scope = DashboardScope.PRIVATE_ELN
         dashboard = DataMgmtServer.get_dashboard_manager(protocol.user).store_dashboard_definition(dashboard)
-        eln_manager, new_entry = _get_entry_creation_criteria(data_type_name,
-                                                              protocol, step_name, ElnEntryType.Dashboard)
+        eln_manager, new_entry = _get_entry_creation_criteria("",protocol, step_name, ElnEntryType.Dashboard)
         # noinspection PyTypeChecker
         update_criteria = ElnDashboardEntryUpdateCriteria()
         update_criteria.dashboard_guid = dashboard.dashboard_guid
         update_criteria.data_source_entry_id = data_source_step.get_id()
         update_criteria.entry_height = 500
         eln_manager.update_experiment_entry(protocol.eln_experiment.notebook_experiment_id, new_entry.entry_id,
                                             update_criteria)
@@ -164,16 +164,41 @@
         chart.grouping_type_data_type_name = data_type_name
         chart.grouping_type_data_field_name = x_field_name
         series.operation_type = operation_type
         series.data_type_name = data_type_name
         series.data_field_name = y_field_name
         chart.series_list = [series]
 
-        dashboard, step = ELNStepFactory._create_dashboard_step_from_chart(chart, data_source_step, data_type_name,
-                                                                           protocol, step_name)
+        dashboard, step = ELNStepFactory._create_dashboard_step_from_chart(chart, data_source_step, protocol, step_name)
+        protocol.invalidate()
+        return step, dashboard
+
+    @staticmethod
+    def create_gantt_chart_step(protocol: ElnExperimentProtocol, data_source_step: ElnEntryStep, step_name: str,
+                                name_field_name: str, start_field_name: str, end_field_name: str,
+                                group_by_field_name: str = "DataRecordName") -> \
+            Tuple[ElnEntryStep, DashboardDefinition]:
+        """
+        Create a gantt chart where start and end are numeric and name is text field.
+
+        In this call, the "group by field" is the label on the left, while the segment name is the one showing on hover
+        of the highlighted region.
+        """
+        if not data_source_step.get_data_type_names():
+            raise ValueError("The data source step did not declare a data type name.")
+        data_type_name: str = data_source_step.get_data_type_names()[0]
+        series: GanttChartSeries = GanttChartSeries(data_type_name, name_field_name,
+                                                    data_type_name, start_field_name,
+                                                    data_type_name, end_field_name)
+        chart = GanttChartDefinition()
+        chart.series_list = [series]
+        chart.grouping_type = ChartGroupingType.GROUP_BY_FIELD
+        chart.grouping_type_data_type_name = data_type_name
+        chart.grouping_type_data_field_name = group_by_field_name
+        dashboard, step = ELNStepFactory._create_dashboard_step_from_chart(chart, data_source_step, protocol, step_name)
         protocol.invalidate()
         return step, dashboard
 
     @staticmethod
     def create_xy_chart_step(protocol: ElnExperimentProtocol, data_source_step: ElnEntryStep, step_name: str,
                              x_field_name: str, y_field_name: str,
                              line_style: LineStyleType = LineStyleType.NORMAL,
@@ -187,16 +212,15 @@
         data_type_name: str = data_source_step.get_data_type_names()[0]
         series: XyChartSeries = XyChartSeries(data_type_name, x_field_name, data_type_name, y_field_name)
         series.line_style_type = line_style
         series.point_shape_type = point_shape
         chart: XyChartDefinition = XyChartDefinition()
         chart.series_list = [series]
 
-        dashboard, step = ELNStepFactory._create_dashboard_step_from_chart(chart, data_source_step, data_type_name,
-                                                                           protocol, step_name)
+        dashboard, step = ELNStepFactory._create_dashboard_step_from_chart(chart, data_source_step, protocol, step_name)
         protocol.invalidate()
         return step, dashboard
 
     @staticmethod
     def create_heatmap_chart_step(protocol: ElnExperimentProtocol, data_source_step: ElnEntryStep, step_name: str,
                                   x_field_name: str, y_field_name: str, size_field_name: Optional[str],
                                   color_field_name: Optional[str], show_data_point_labels: bool = True,
@@ -212,16 +236,15 @@
                                                         data_type_name, size_field_name,
                                                         data_type_name, color_field_name)
         series.show_data_point_labels = show_data_point_labels
         chart: HeatMapChartDefinition = HeatMapChartDefinition()
         chart.min_number_of_rows = min_num_rows
         chart.min_number_of_cols = min_num_cols
 
-        dashboard, step = ELNStepFactory._create_dashboard_step_from_chart(chart, data_source_step, data_type_name,
-                                                                           protocol, step_name)
+        dashboard, step = ELNStepFactory._create_dashboard_step_from_chart(chart, data_source_step, protocol, step_name)
         protocol.invalidate()
         return step, dashboard
 
     @staticmethod
     def add_3d_plate_step(protocol: ElnExperimentProtocol, layers: List[MultiLayerPlateLayer],
                           config: MultiLayerPlateConfig = MultiLayerPlateConfig(),
                           entry_name: str = "3D Plating") -> Tuple[ElnEntryStep, List[DataRecord], List[DataRecord]]:
```

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/LICENSE` & `sapiopylib-2023.6.7.141/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/README.md` & `sapiopylib-2023.6.7.141/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.6.140/pyproject.toml` & `sapiopylib-2023.6.7.141/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.06.06.140'
+version='2023.06.07.141'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sapiopylib-2023.6.6.140/PKG-INFO` & `sapiopylib-2023.6.7.141/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.6.6.140
+Version: 2023.6.7.141
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

