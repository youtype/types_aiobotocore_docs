# Literals

> [Index](../README.md) > [QuickSight](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## AnalysisErrorTypeType

```python
# AnalysisErrorTypeType usage example

from types_aiobotocore_quicksight.literals import AnalysisErrorTypeType

def get_value() -> AnalysisErrorTypeType:
    return "ACCESS_DENIED"
```

```python
# AnalysisErrorTypeType definition

AnalysisErrorTypeType = Literal[
    "ACCESS_DENIED",
    "COLUMN_GEOGRAPHIC_ROLE_MISMATCH",
    "COLUMN_REPLACEMENT_MISSING",
    "COLUMN_TYPE_MISMATCH",
    "DATA_SET_NOT_FOUND",
    "INTERNAL_FAILURE",
    "PARAMETER_NOT_FOUND",
    "PARAMETER_TYPE_INVALID",
    "PARAMETER_VALUE_INCOMPATIBLE",
    "SOURCE_NOT_FOUND",
]
```
## AnalysisFilterAttributeType

```python
# AnalysisFilterAttributeType usage example

from types_aiobotocore_quicksight.literals import AnalysisFilterAttributeType

def get_value() -> AnalysisFilterAttributeType:
    return "ANALYSIS_NAME"
```

```python
# AnalysisFilterAttributeType definition

AnalysisFilterAttributeType = Literal[
    "ANALYSIS_NAME",
    "DIRECT_QUICKSIGHT_OWNER",
    "DIRECT_QUICKSIGHT_SOLE_OWNER",
    "DIRECT_QUICKSIGHT_VIEWER_OR_OWNER",
    "QUICKSIGHT_OWNER",
    "QUICKSIGHT_USER",
    "QUICKSIGHT_VIEWER_OR_OWNER",
]
```
## AnchorOptionType

```python
# AnchorOptionType usage example

from types_aiobotocore_quicksight.literals import AnchorOptionType

def get_value() -> AnchorOptionType:
    return "NOW"
```

```python
# AnchorOptionType definition

AnchorOptionType = Literal[
    "NOW",
]
```
## ArcThicknessOptionsType

```python
# ArcThicknessOptionsType usage example

from types_aiobotocore_quicksight.literals import ArcThicknessOptionsType

def get_value() -> ArcThicknessOptionsType:
    return "LARGE"
```

```python
# ArcThicknessOptionsType definition

ArcThicknessOptionsType = Literal[
    "LARGE",
    "MEDIUM",
    "SMALL",
]
```
## ArcThicknessType

```python
# ArcThicknessType usage example

from types_aiobotocore_quicksight.literals import ArcThicknessType

def get_value() -> ArcThicknessType:
    return "LARGE"
```

```python
# ArcThicknessType definition

ArcThicknessType = Literal[
    "LARGE",
    "MEDIUM",
    "SMALL",
    "WHOLE",
]
```
## AssetBundleExportFormatType

```python
# AssetBundleExportFormatType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportFormatType

def get_value() -> AssetBundleExportFormatType:
    return "CLOUDFORMATION_JSON"
```

```python
# AssetBundleExportFormatType definition

AssetBundleExportFormatType = Literal[
    "CLOUDFORMATION_JSON",
    "QUICKSIGHT_JSON",
]
```
## AssetBundleExportJobAnalysisPropertyToOverrideType

```python
# AssetBundleExportJobAnalysisPropertyToOverrideType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobAnalysisPropertyToOverrideType

def get_value() -> AssetBundleExportJobAnalysisPropertyToOverrideType:
    return "Name"
```

```python
# AssetBundleExportJobAnalysisPropertyToOverrideType definition

AssetBundleExportJobAnalysisPropertyToOverrideType = Literal[
    "Name",
]
```
## AssetBundleExportJobDashboardPropertyToOverrideType

```python
# AssetBundleExportJobDashboardPropertyToOverrideType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobDashboardPropertyToOverrideType

def get_value() -> AssetBundleExportJobDashboardPropertyToOverrideType:
    return "Name"
```

```python
# AssetBundleExportJobDashboardPropertyToOverrideType definition

AssetBundleExportJobDashboardPropertyToOverrideType = Literal[
    "Name",
]
```
## AssetBundleExportJobDataSetPropertyToOverrideType

```python
# AssetBundleExportJobDataSetPropertyToOverrideType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobDataSetPropertyToOverrideType

def get_value() -> AssetBundleExportJobDataSetPropertyToOverrideType:
    return "Name"
```

```python
# AssetBundleExportJobDataSetPropertyToOverrideType definition

AssetBundleExportJobDataSetPropertyToOverrideType = Literal[
    "Name",
]
```
## AssetBundleExportJobDataSourcePropertyToOverrideType

```python
# AssetBundleExportJobDataSourcePropertyToOverrideType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobDataSourcePropertyToOverrideType

def get_value() -> AssetBundleExportJobDataSourcePropertyToOverrideType:
    return "Catalog"
```

```python
# AssetBundleExportJobDataSourcePropertyToOverrideType definition

AssetBundleExportJobDataSourcePropertyToOverrideType = Literal[
    "Catalog",
    "ClusterId",
    "Database",
    "DataSetName",
    "DisableSsl",
    "Domain",
    "Host",
    "InstanceId",
    "ManifestFileLocation",
    "Name",
    "Password",
    "Port",
    "RoleArn",
    "SecretArn",
    "Username",
    "Warehouse",
    "WorkGroup",
]
```
## AssetBundleExportJobRefreshSchedulePropertyToOverrideType

```python
# AssetBundleExportJobRefreshSchedulePropertyToOverrideType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobRefreshSchedulePropertyToOverrideType

def get_value() -> AssetBundleExportJobRefreshSchedulePropertyToOverrideType:
    return "StartAfterDateTime"
```

```python
# AssetBundleExportJobRefreshSchedulePropertyToOverrideType definition

AssetBundleExportJobRefreshSchedulePropertyToOverrideType = Literal[
    "StartAfterDateTime",
]
```
## AssetBundleExportJobStatusType

```python
# AssetBundleExportJobStatusType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobStatusType

def get_value() -> AssetBundleExportJobStatusType:
    return "FAILED"
```

```python
# AssetBundleExportJobStatusType definition

AssetBundleExportJobStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "QUEUED_FOR_IMMEDIATE_EXECUTION",
    "SUCCESSFUL",
]
```
## AssetBundleExportJobThemePropertyToOverrideType

```python
# AssetBundleExportJobThemePropertyToOverrideType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobThemePropertyToOverrideType

def get_value() -> AssetBundleExportJobThemePropertyToOverrideType:
    return "Name"
```

```python
# AssetBundleExportJobThemePropertyToOverrideType definition

AssetBundleExportJobThemePropertyToOverrideType = Literal[
    "Name",
]
```
## AssetBundleExportJobVPCConnectionPropertyToOverrideType

```python
# AssetBundleExportJobVPCConnectionPropertyToOverrideType usage example

from types_aiobotocore_quicksight.literals import AssetBundleExportJobVPCConnectionPropertyToOverrideType

def get_value() -> AssetBundleExportJobVPCConnectionPropertyToOverrideType:
    return "DnsResolvers"
```

```python
# AssetBundleExportJobVPCConnectionPropertyToOverrideType definition

AssetBundleExportJobVPCConnectionPropertyToOverrideType = Literal[
    "DnsResolvers",
    "Name",
    "RoleArn",
]
```
## AssetBundleImportFailureActionType

```python
# AssetBundleImportFailureActionType usage example

from types_aiobotocore_quicksight.literals import AssetBundleImportFailureActionType

def get_value() -> AssetBundleImportFailureActionType:
    return "DO_NOTHING"
```

```python
# AssetBundleImportFailureActionType definition

AssetBundleImportFailureActionType = Literal[
    "DO_NOTHING",
    "ROLLBACK",
]
```
## AssetBundleImportJobStatusType

```python
# AssetBundleImportJobStatusType usage example

from types_aiobotocore_quicksight.literals import AssetBundleImportJobStatusType

def get_value() -> AssetBundleImportJobStatusType:
    return "FAILED"
```

```python
# AssetBundleImportJobStatusType definition

AssetBundleImportJobStatusType = Literal[
    "FAILED",
    "FAILED_ROLLBACK_COMPLETED",
    "FAILED_ROLLBACK_ERROR",
    "FAILED_ROLLBACK_IN_PROGRESS",
    "IN_PROGRESS",
    "QUEUED_FOR_IMMEDIATE_EXECUTION",
    "SUCCESSFUL",
]
```
## AssignmentStatusType

```python
# AssignmentStatusType usage example

from types_aiobotocore_quicksight.literals import AssignmentStatusType

def get_value() -> AssignmentStatusType:
    return "DISABLED"
```

```python
# AssignmentStatusType definition

AssignmentStatusType = Literal[
    "DISABLED",
    "DRAFT",
    "ENABLED",
]
```
## AuthenticationMethodOptionType

```python
# AuthenticationMethodOptionType usage example

from types_aiobotocore_quicksight.literals import AuthenticationMethodOptionType

def get_value() -> AuthenticationMethodOptionType:
    return "ACTIVE_DIRECTORY"
```

```python
# AuthenticationMethodOptionType definition

AuthenticationMethodOptionType = Literal[
    "ACTIVE_DIRECTORY",
    "IAM_AND_QUICKSIGHT",
    "IAM_IDENTITY_CENTER",
    "IAM_ONLY",
]
```
## AuthorSpecifiedAggregationType

```python
# AuthorSpecifiedAggregationType usage example

from types_aiobotocore_quicksight.literals import AuthorSpecifiedAggregationType

def get_value() -> AuthorSpecifiedAggregationType:
    return "AVERAGE"
```

```python
# AuthorSpecifiedAggregationType definition

AuthorSpecifiedAggregationType = Literal[
    "AVERAGE",
    "COUNT",
    "DISTINCT_COUNT",
    "MAX",
    "MEDIAN",
    "MIN",
    "PERCENTILE",
    "STDEV",
    "STDEVP",
    "SUM",
    "VAR",
    "VARP",
]
```
## AxisBindingType

```python
# AxisBindingType usage example

from types_aiobotocore_quicksight.literals import AxisBindingType

def get_value() -> AxisBindingType:
    return "PRIMARY_YAXIS"
```

```python
# AxisBindingType definition

AxisBindingType = Literal[
    "PRIMARY_YAXIS",
    "SECONDARY_YAXIS",
]
```
## BarChartOrientationType

```python
# BarChartOrientationType usage example

from types_aiobotocore_quicksight.literals import BarChartOrientationType

def get_value() -> BarChartOrientationType:
    return "HORIZONTAL"
```

```python
# BarChartOrientationType definition

BarChartOrientationType = Literal[
    "HORIZONTAL",
    "VERTICAL",
]
```
## BarsArrangementType

```python
# BarsArrangementType usage example

from types_aiobotocore_quicksight.literals import BarsArrangementType

def get_value() -> BarsArrangementType:
    return "CLUSTERED"
```

```python
# BarsArrangementType definition

BarsArrangementType = Literal[
    "CLUSTERED",
    "STACKED",
    "STACKED_PERCENT",
]
```
## BaseMapStyleTypeType

```python
# BaseMapStyleTypeType usage example

from types_aiobotocore_quicksight.literals import BaseMapStyleTypeType

def get_value() -> BaseMapStyleTypeType:
    return "DARK_GRAY"
```

```python
# BaseMapStyleTypeType definition

BaseMapStyleTypeType = Literal[
    "DARK_GRAY",
    "IMAGERY",
    "LIGHT_GRAY",
    "STREET",
]
```
## BoxPlotFillStyleType

```python
# BoxPlotFillStyleType usage example

from types_aiobotocore_quicksight.literals import BoxPlotFillStyleType

def get_value() -> BoxPlotFillStyleType:
    return "SOLID"
```

```python
# BoxPlotFillStyleType definition

BoxPlotFillStyleType = Literal[
    "SOLID",
    "TRANSPARENT",
]
```
## CategoricalAggregationFunctionType

```python
# CategoricalAggregationFunctionType usage example

from types_aiobotocore_quicksight.literals import CategoricalAggregationFunctionType

def get_value() -> CategoricalAggregationFunctionType:
    return "COUNT"
```

```python
# CategoricalAggregationFunctionType definition

CategoricalAggregationFunctionType = Literal[
    "COUNT",
    "DISTINCT_COUNT",
]
```
## CategoryFilterFunctionType

```python
# CategoryFilterFunctionType usage example

from types_aiobotocore_quicksight.literals import CategoryFilterFunctionType

def get_value() -> CategoryFilterFunctionType:
    return "CONTAINS"
```

```python
# CategoryFilterFunctionType definition

CategoryFilterFunctionType = Literal[
    "CONTAINS",
    "EXACT",
]
```
## CategoryFilterMatchOperatorType

```python
# CategoryFilterMatchOperatorType usage example

from types_aiobotocore_quicksight.literals import CategoryFilterMatchOperatorType

def get_value() -> CategoryFilterMatchOperatorType:
    return "CONTAINS"
```

```python
# CategoryFilterMatchOperatorType definition

CategoryFilterMatchOperatorType = Literal[
    "CONTAINS",
    "DOES_NOT_CONTAIN",
    "DOES_NOT_EQUAL",
    "ENDS_WITH",
    "EQUALS",
    "STARTS_WITH",
]
```
## CategoryFilterSelectAllOptionsType

```python
# CategoryFilterSelectAllOptionsType usage example

from types_aiobotocore_quicksight.literals import CategoryFilterSelectAllOptionsType

def get_value() -> CategoryFilterSelectAllOptionsType:
    return "FILTER_ALL_VALUES"
```

```python
# CategoryFilterSelectAllOptionsType definition

CategoryFilterSelectAllOptionsType = Literal[
    "FILTER_ALL_VALUES",
]
```
## CategoryFilterTypeType

```python
# CategoryFilterTypeType usage example

from types_aiobotocore_quicksight.literals import CategoryFilterTypeType

def get_value() -> CategoryFilterTypeType:
    return "CUSTOM_FILTER"
```

```python
# CategoryFilterTypeType definition

CategoryFilterTypeType = Literal[
    "CUSTOM_FILTER",
    "CUSTOM_FILTER_LIST",
    "FILTER_LIST",
]
```
## ColorFillTypeType

```python
# ColorFillTypeType usage example

from types_aiobotocore_quicksight.literals import ColorFillTypeType

def get_value() -> ColorFillTypeType:
    return "DISCRETE"
```

```python
# ColorFillTypeType definition

ColorFillTypeType = Literal[
    "DISCRETE",
    "GRADIENT",
]
```
## ColumnDataRoleType

```python
# ColumnDataRoleType usage example

from types_aiobotocore_quicksight.literals import ColumnDataRoleType

def get_value() -> ColumnDataRoleType:
    return "DIMENSION"
```

```python
# ColumnDataRoleType definition

ColumnDataRoleType = Literal[
    "DIMENSION",
    "MEASURE",
]
```
## ColumnDataTypeType

```python
# ColumnDataTypeType usage example

from types_aiobotocore_quicksight.literals import ColumnDataTypeType

def get_value() -> ColumnDataTypeType:
    return "DATETIME"
```

```python
# ColumnDataTypeType definition

ColumnDataTypeType = Literal[
    "DATETIME",
    "DECIMAL",
    "INTEGER",
    "STRING",
]
```
## ColumnOrderingTypeType

```python
# ColumnOrderingTypeType usage example

from types_aiobotocore_quicksight.literals import ColumnOrderingTypeType

def get_value() -> ColumnOrderingTypeType:
    return "GREATER_IS_BETTER"
```

```python
# ColumnOrderingTypeType definition

ColumnOrderingTypeType = Literal[
    "GREATER_IS_BETTER",
    "LESSER_IS_BETTER",
    "SPECIFIED",
]
```
## ColumnRoleType

```python
# ColumnRoleType usage example

from types_aiobotocore_quicksight.literals import ColumnRoleType

def get_value() -> ColumnRoleType:
    return "DIMENSION"
```

```python
# ColumnRoleType definition

ColumnRoleType = Literal[
    "DIMENSION",
    "MEASURE",
]
```
## ColumnTagNameType

```python
# ColumnTagNameType usage example

from types_aiobotocore_quicksight.literals import ColumnTagNameType

def get_value() -> ColumnTagNameType:
    return "COLUMN_DESCRIPTION"
```

```python
# ColumnTagNameType definition

ColumnTagNameType = Literal[
    "COLUMN_DESCRIPTION",
    "COLUMN_GEOGRAPHIC_ROLE",
]
```
## ComparisonMethodType

```python
# ComparisonMethodType usage example

from types_aiobotocore_quicksight.literals import ComparisonMethodType

def get_value() -> ComparisonMethodType:
    return "DIFFERENCE"
```

```python
# ComparisonMethodType definition

ComparisonMethodType = Literal[
    "DIFFERENCE",
    "PERCENT",
    "PERCENT_DIFFERENCE",
]
```
## ConditionalFormattingIconDisplayOptionType

```python
# ConditionalFormattingIconDisplayOptionType usage example

from types_aiobotocore_quicksight.literals import ConditionalFormattingIconDisplayOptionType

def get_value() -> ConditionalFormattingIconDisplayOptionType:
    return "ICON_ONLY"
```

```python
# ConditionalFormattingIconDisplayOptionType definition

ConditionalFormattingIconDisplayOptionType = Literal[
    "ICON_ONLY",
]
```
## ConditionalFormattingIconSetTypeType

```python
# ConditionalFormattingIconSetTypeType usage example

from types_aiobotocore_quicksight.literals import ConditionalFormattingIconSetTypeType

def get_value() -> ConditionalFormattingIconSetTypeType:
    return "BARS"
```

```python
# ConditionalFormattingIconSetTypeType definition

ConditionalFormattingIconSetTypeType = Literal[
    "BARS",
    "CARET_UP_MINUS_DOWN",
    "CHECK_X",
    "FLAGS",
    "FOUR_COLOR_ARROW",
    "FOUR_GRAY_ARROW",
    "PLUS_MINUS",
    "THREE_CIRCLE",
    "THREE_COLOR_ARROW",
    "THREE_GRAY_ARROW",
    "THREE_SHAPE",
]
```
## ConstantTypeType

```python
# ConstantTypeType usage example

from types_aiobotocore_quicksight.literals import ConstantTypeType

def get_value() -> ConstantTypeType:
    return "COLLECTIVE"
```

```python
# ConstantTypeType definition

ConstantTypeType = Literal[
    "COLLECTIVE",
    "RANGE",
    "SINGULAR",
]
```
## CrossDatasetTypesType

```python
# CrossDatasetTypesType usage example

from types_aiobotocore_quicksight.literals import CrossDatasetTypesType

def get_value() -> CrossDatasetTypesType:
    return "ALL_DATASETS"
```

```python
# CrossDatasetTypesType definition

CrossDatasetTypesType = Literal[
    "ALL_DATASETS",
    "SINGLE_DATASET",
]
```
## CustomContentImageScalingConfigurationType

```python
# CustomContentImageScalingConfigurationType usage example

from types_aiobotocore_quicksight.literals import CustomContentImageScalingConfigurationType

def get_value() -> CustomContentImageScalingConfigurationType:
    return "DO_NOT_SCALE"
```

```python
# CustomContentImageScalingConfigurationType definition

CustomContentImageScalingConfigurationType = Literal[
    "DO_NOT_SCALE",
    "FIT_TO_HEIGHT",
    "FIT_TO_WIDTH",
    "SCALE_TO_VISUAL",
]
```
## CustomContentTypeType

```python
# CustomContentTypeType usage example

from types_aiobotocore_quicksight.literals import CustomContentTypeType

def get_value() -> CustomContentTypeType:
    return "IMAGE"
```

```python
# CustomContentTypeType definition

CustomContentTypeType = Literal[
    "IMAGE",
    "OTHER_EMBEDDED_CONTENT",
]
```
## DashboardBehaviorType

```python
# DashboardBehaviorType usage example

from types_aiobotocore_quicksight.literals import DashboardBehaviorType

def get_value() -> DashboardBehaviorType:
    return "DISABLED"
```

```python
# DashboardBehaviorType definition

DashboardBehaviorType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## DashboardErrorTypeType

```python
# DashboardErrorTypeType usage example

from types_aiobotocore_quicksight.literals import DashboardErrorTypeType

def get_value() -> DashboardErrorTypeType:
    return "ACCESS_DENIED"
```

```python
# DashboardErrorTypeType definition

DashboardErrorTypeType = Literal[
    "ACCESS_DENIED",
    "COLUMN_GEOGRAPHIC_ROLE_MISMATCH",
    "COLUMN_REPLACEMENT_MISSING",
    "COLUMN_TYPE_MISMATCH",
    "DATA_SET_NOT_FOUND",
    "INTERNAL_FAILURE",
    "PARAMETER_NOT_FOUND",
    "PARAMETER_TYPE_INVALID",
    "PARAMETER_VALUE_INCOMPATIBLE",
    "SOURCE_NOT_FOUND",
]
```
## DashboardFilterAttributeType

```python
# DashboardFilterAttributeType usage example

from types_aiobotocore_quicksight.literals import DashboardFilterAttributeType

def get_value() -> DashboardFilterAttributeType:
    return "DASHBOARD_NAME"
```

```python
# DashboardFilterAttributeType definition

DashboardFilterAttributeType = Literal[
    "DASHBOARD_NAME",
    "DIRECT_QUICKSIGHT_OWNER",
    "DIRECT_QUICKSIGHT_SOLE_OWNER",
    "DIRECT_QUICKSIGHT_VIEWER_OR_OWNER",
    "QUICKSIGHT_OWNER",
    "QUICKSIGHT_USER",
    "QUICKSIGHT_VIEWER_OR_OWNER",
]
```
## DashboardUIStateType

```python
# DashboardUIStateType usage example

from types_aiobotocore_quicksight.literals import DashboardUIStateType

def get_value() -> DashboardUIStateType:
    return "COLLAPSED"
```

```python
# DashboardUIStateType definition

DashboardUIStateType = Literal[
    "COLLAPSED",
    "EXPANDED",
]
```
## DataLabelContentType

```python
# DataLabelContentType usage example

from types_aiobotocore_quicksight.literals import DataLabelContentType

def get_value() -> DataLabelContentType:
    return "PERCENT"
```

```python
# DataLabelContentType definition

DataLabelContentType = Literal[
    "PERCENT",
    "VALUE",
    "VALUE_AND_PERCENT",
]
```
## DataLabelOverlapType

```python
# DataLabelOverlapType usage example

from types_aiobotocore_quicksight.literals import DataLabelOverlapType

def get_value() -> DataLabelOverlapType:
    return "DISABLE_OVERLAP"
```

```python
# DataLabelOverlapType definition

DataLabelOverlapType = Literal[
    "DISABLE_OVERLAP",
    "ENABLE_OVERLAP",
]
```
## DataLabelPositionType

```python
# DataLabelPositionType usage example

from types_aiobotocore_quicksight.literals import DataLabelPositionType

def get_value() -> DataLabelPositionType:
    return "BOTTOM"
```

```python
# DataLabelPositionType definition

DataLabelPositionType = Literal[
    "BOTTOM",
    "INSIDE",
    "LEFT",
    "OUTSIDE",
    "RIGHT",
    "TOP",
]
```
## DataSetFilterAttributeType

```python
# DataSetFilterAttributeType usage example

from types_aiobotocore_quicksight.literals import DataSetFilterAttributeType

def get_value() -> DataSetFilterAttributeType:
    return "DATASET_NAME"
```

```python
# DataSetFilterAttributeType definition

DataSetFilterAttributeType = Literal[
    "DATASET_NAME",
    "DIRECT_QUICKSIGHT_OWNER",
    "DIRECT_QUICKSIGHT_SOLE_OWNER",
    "DIRECT_QUICKSIGHT_VIEWER_OR_OWNER",
    "QUICKSIGHT_OWNER",
    "QUICKSIGHT_VIEWER_OR_OWNER",
]
```
## DataSetImportModeType

```python
# DataSetImportModeType usage example

from types_aiobotocore_quicksight.literals import DataSetImportModeType

def get_value() -> DataSetImportModeType:
    return "DIRECT_QUERY"
```

```python
# DataSetImportModeType definition

DataSetImportModeType = Literal[
    "DIRECT_QUERY",
    "SPICE",
]
```
## DataSourceErrorInfoTypeType

```python
# DataSourceErrorInfoTypeType usage example

from types_aiobotocore_quicksight.literals import DataSourceErrorInfoTypeType

def get_value() -> DataSourceErrorInfoTypeType:
    return "ACCESS_DENIED"
```

```python
# DataSourceErrorInfoTypeType definition

DataSourceErrorInfoTypeType = Literal[
    "ACCESS_DENIED",
    "CONFLICT",
    "COPY_SOURCE_NOT_FOUND",
    "ENGINE_VERSION_NOT_SUPPORTED",
    "GENERIC_SQL_FAILURE",
    "TIMEOUT",
    "UNKNOWN",
    "UNKNOWN_HOST",
]
```
## DataSourceFilterAttributeType

```python
# DataSourceFilterAttributeType usage example

from types_aiobotocore_quicksight.literals import DataSourceFilterAttributeType

def get_value() -> DataSourceFilterAttributeType:
    return "DATASOURCE_NAME"
```

```python
# DataSourceFilterAttributeType definition

DataSourceFilterAttributeType = Literal[
    "DATASOURCE_NAME",
    "DIRECT_QUICKSIGHT_OWNER",
    "DIRECT_QUICKSIGHT_SOLE_OWNER",
    "DIRECT_QUICKSIGHT_VIEWER_OR_OWNER",
]
```
## DataSourceTypeType

```python
# DataSourceTypeType usage example

from types_aiobotocore_quicksight.literals import DataSourceTypeType

def get_value() -> DataSourceTypeType:
    return "ADOBE_ANALYTICS"
```

```python
# DataSourceTypeType definition

DataSourceTypeType = Literal[
    "ADOBE_ANALYTICS",
    "AMAZON_ELASTICSEARCH",
    "AMAZON_OPENSEARCH",
    "ATHENA",
    "AURORA",
    "AURORA_POSTGRESQL",
    "AWS_IOT_ANALYTICS",
    "DATABRICKS",
    "EXASOL",
    "GITHUB",
    "JIRA",
    "MARIADB",
    "MYSQL",
    "ORACLE",
    "POSTGRESQL",
    "PRESTO",
    "REDSHIFT",
    "S3",
    "SALESFORCE",
    "SERVICENOW",
    "SNOWFLAKE",
    "SPARK",
    "SQLSERVER",
    "TERADATA",
    "TIMESTREAM",
    "TWITTER",
]
```
## DatasetParameterValueTypeType

```python
# DatasetParameterValueTypeType usage example

from types_aiobotocore_quicksight.literals import DatasetParameterValueTypeType

def get_value() -> DatasetParameterValueTypeType:
    return "MULTI_VALUED"
```

```python
# DatasetParameterValueTypeType definition

DatasetParameterValueTypeType = Literal[
    "MULTI_VALUED",
    "SINGLE_VALUED",
]
```
## DateAggregationFunctionType

```python
# DateAggregationFunctionType usage example

from types_aiobotocore_quicksight.literals import DateAggregationFunctionType

def get_value() -> DateAggregationFunctionType:
    return "COUNT"
```

```python
# DateAggregationFunctionType definition

DateAggregationFunctionType = Literal[
    "COUNT",
    "DISTINCT_COUNT",
    "MAX",
    "MIN",
]
```
## DayOfWeekType

```python
# DayOfWeekType usage example

from types_aiobotocore_quicksight.literals import DayOfWeekType

def get_value() -> DayOfWeekType:
    return "FRIDAY"
```

```python
# DayOfWeekType definition

DayOfWeekType = Literal[
    "FRIDAY",
    "MONDAY",
    "SATURDAY",
    "SUNDAY",
    "THURSDAY",
    "TUESDAY",
    "WEDNESDAY",
]
```
## DefaultAggregationType

```python
# DefaultAggregationType usage example

from types_aiobotocore_quicksight.literals import DefaultAggregationType

def get_value() -> DefaultAggregationType:
    return "AVERAGE"
```

```python
# DefaultAggregationType definition

DefaultAggregationType = Literal[
    "AVERAGE",
    "COUNT",
    "DISTINCT_COUNT",
    "MAX",
    "MEDIAN",
    "MIN",
    "STDEV",
    "STDEVP",
    "SUM",
    "VAR",
    "VARP",
]
```
## DisplayFormatType

```python
# DisplayFormatType usage example

from types_aiobotocore_quicksight.literals import DisplayFormatType

def get_value() -> DisplayFormatType:
    return "AUTO"
```

```python
# DisplayFormatType definition

DisplayFormatType = Literal[
    "AUTO",
    "CURRENCY",
    "DATE",
    "NUMBER",
    "PERCENT",
    "STRING",
]
```
## EditionType

```python
# EditionType usage example

from types_aiobotocore_quicksight.literals import EditionType

def get_value() -> EditionType:
    return "ENTERPRISE"
```

```python
# EditionType definition

EditionType = Literal[
    "ENTERPRISE",
    "ENTERPRISE_AND_Q",
    "STANDARD",
]
```
## EmbeddingIdentityTypeType

```python
# EmbeddingIdentityTypeType usage example

from types_aiobotocore_quicksight.literals import EmbeddingIdentityTypeType

def get_value() -> EmbeddingIdentityTypeType:
    return "ANONYMOUS"
```

```python
# EmbeddingIdentityTypeType definition

EmbeddingIdentityTypeType = Literal[
    "ANONYMOUS",
    "IAM",
    "QUICKSIGHT",
]
```
## FileFormatType

```python
# FileFormatType usage example

from types_aiobotocore_quicksight.literals import FileFormatType

def get_value() -> FileFormatType:
    return "CLF"
```

```python
# FileFormatType definition

FileFormatType = Literal[
    "CLF",
    "CSV",
    "ELF",
    "JSON",
    "TSV",
    "XLSX",
]
```
## FilterClassType

```python
# FilterClassType usage example

from types_aiobotocore_quicksight.literals import FilterClassType

def get_value() -> FilterClassType:
    return "CONDITIONAL_VALUE_FILTER"
```

```python
# FilterClassType definition

FilterClassType = Literal[
    "CONDITIONAL_VALUE_FILTER",
    "ENFORCED_VALUE_FILTER",
    "NAMED_VALUE_FILTER",
]
```
## FilterNullOptionType

```python
# FilterNullOptionType usage example

from types_aiobotocore_quicksight.literals import FilterNullOptionType

def get_value() -> FilterNullOptionType:
    return "ALL_VALUES"
```

```python
# FilterNullOptionType definition

FilterNullOptionType = Literal[
    "ALL_VALUES",
    "NON_NULLS_ONLY",
    "NULLS_ONLY",
]
```
## FilterOperatorType

```python
# FilterOperatorType usage example

from types_aiobotocore_quicksight.literals import FilterOperatorType

def get_value() -> FilterOperatorType:
    return "StringEquals"
```

```python
# FilterOperatorType definition

FilterOperatorType = Literal[
    "StringEquals",
    "StringLike",
]
```
## FilterVisualScopeType

```python
# FilterVisualScopeType usage example

from types_aiobotocore_quicksight.literals import FilterVisualScopeType

def get_value() -> FilterVisualScopeType:
    return "ALL_VISUALS"
```

```python
# FilterVisualScopeType definition

FilterVisualScopeType = Literal[
    "ALL_VISUALS",
    "SELECTED_VISUALS",
]
```
## FolderFilterAttributeType

```python
# FolderFilterAttributeType usage example

from types_aiobotocore_quicksight.literals import FolderFilterAttributeType

def get_value() -> FolderFilterAttributeType:
    return "DIRECT_QUICKSIGHT_OWNER"
```

```python
# FolderFilterAttributeType definition

FolderFilterAttributeType = Literal[
    "DIRECT_QUICKSIGHT_OWNER",
    "DIRECT_QUICKSIGHT_SOLE_OWNER",
    "DIRECT_QUICKSIGHT_VIEWER_OR_OWNER",
    "FOLDER_NAME",
    "PARENT_FOLDER_ARN",
    "QUICKSIGHT_OWNER",
    "QUICKSIGHT_VIEWER_OR_OWNER",
]
```
## FolderTypeType

```python
# FolderTypeType usage example

from types_aiobotocore_quicksight.literals import FolderTypeType

def get_value() -> FolderTypeType:
    return "SHARED"
```

```python
# FolderTypeType definition

FolderTypeType = Literal[
    "SHARED",
]
```
## FontDecorationType

```python
# FontDecorationType usage example

from types_aiobotocore_quicksight.literals import FontDecorationType

def get_value() -> FontDecorationType:
    return "NONE"
```

```python
# FontDecorationType definition

FontDecorationType = Literal[
    "NONE",
    "UNDERLINE",
]
```
## FontStyleType

```python
# FontStyleType usage example

from types_aiobotocore_quicksight.literals import FontStyleType

def get_value() -> FontStyleType:
    return "ITALIC"
```

```python
# FontStyleType definition

FontStyleType = Literal[
    "ITALIC",
    "NORMAL",
]
```
## FontWeightNameType

```python
# FontWeightNameType usage example

from types_aiobotocore_quicksight.literals import FontWeightNameType

def get_value() -> FontWeightNameType:
    return "BOLD"
```

```python
# FontWeightNameType definition

FontWeightNameType = Literal[
    "BOLD",
    "NORMAL",
]
```
## ForecastComputationSeasonalityType

```python
# ForecastComputationSeasonalityType usage example

from types_aiobotocore_quicksight.literals import ForecastComputationSeasonalityType

def get_value() -> ForecastComputationSeasonalityType:
    return "AUTOMATIC"
```

```python
# ForecastComputationSeasonalityType definition

ForecastComputationSeasonalityType = Literal[
    "AUTOMATIC",
    "CUSTOM",
]
```
## FunnelChartMeasureDataLabelStyleType

```python
# FunnelChartMeasureDataLabelStyleType usage example

from types_aiobotocore_quicksight.literals import FunnelChartMeasureDataLabelStyleType

def get_value() -> FunnelChartMeasureDataLabelStyleType:
    return "PERCENTAGE_BY_FIRST_STAGE"
```

```python
# FunnelChartMeasureDataLabelStyleType definition

FunnelChartMeasureDataLabelStyleType = Literal[
    "PERCENTAGE_BY_FIRST_STAGE",
    "PERCENTAGE_BY_PREVIOUS_STAGE",
    "VALUE_AND_PERCENTAGE_BY_FIRST_STAGE",
    "VALUE_AND_PERCENTAGE_BY_PREVIOUS_STAGE",
    "VALUE_ONLY",
]
```
## GeoSpatialCountryCodeType

```python
# GeoSpatialCountryCodeType usage example

from types_aiobotocore_quicksight.literals import GeoSpatialCountryCodeType

def get_value() -> GeoSpatialCountryCodeType:
    return "US"
```

```python
# GeoSpatialCountryCodeType definition

GeoSpatialCountryCodeType = Literal[
    "US",
]
```
## GeoSpatialDataRoleType

```python
# GeoSpatialDataRoleType usage example

from types_aiobotocore_quicksight.literals import GeoSpatialDataRoleType

def get_value() -> GeoSpatialDataRoleType:
    return "CITY"
```

```python
# GeoSpatialDataRoleType definition

GeoSpatialDataRoleType = Literal[
    "CITY",
    "COUNTRY",
    "COUNTY",
    "LATITUDE",
    "LONGITUDE",
    "POSTCODE",
    "STATE",
]
```
## GeospatialSelectedPointStyleType

```python
# GeospatialSelectedPointStyleType usage example

from types_aiobotocore_quicksight.literals import GeospatialSelectedPointStyleType

def get_value() -> GeospatialSelectedPointStyleType:
    return "CLUSTER"
```

```python
# GeospatialSelectedPointStyleType definition

GeospatialSelectedPointStyleType = Literal[
    "CLUSTER",
    "HEATMAP",
    "POINT",
]
```
## GroupFilterAttributeType

```python
# GroupFilterAttributeType usage example

from types_aiobotocore_quicksight.literals import GroupFilterAttributeType

def get_value() -> GroupFilterAttributeType:
    return "GROUP_NAME"
```

```python
# GroupFilterAttributeType definition

GroupFilterAttributeType = Literal[
    "GROUP_NAME",
]
```
## GroupFilterOperatorType

```python
# GroupFilterOperatorType usage example

from types_aiobotocore_quicksight.literals import GroupFilterOperatorType

def get_value() -> GroupFilterOperatorType:
    return "StartsWith"
```

```python
# GroupFilterOperatorType definition

GroupFilterOperatorType = Literal[
    "StartsWith",
]
```
## HistogramBinTypeType

```python
# HistogramBinTypeType usage example

from types_aiobotocore_quicksight.literals import HistogramBinTypeType

def get_value() -> HistogramBinTypeType:
    return "BIN_COUNT"
```

```python
# HistogramBinTypeType definition

HistogramBinTypeType = Literal[
    "BIN_COUNT",
    "BIN_WIDTH",
]
```
## HorizontalTextAlignmentType

```python
# HorizontalTextAlignmentType usage example

from types_aiobotocore_quicksight.literals import HorizontalTextAlignmentType

def get_value() -> HorizontalTextAlignmentType:
    return "AUTO"
```

```python
# HorizontalTextAlignmentType definition

HorizontalTextAlignmentType = Literal[
    "AUTO",
    "CENTER",
    "LEFT",
    "RIGHT",
]
```
## IconType

```python
# IconType usage example

from types_aiobotocore_quicksight.literals import IconType

def get_value() -> IconType:
    return "ARROW_DOWN"
```

```python
# IconType definition

IconType = Literal[
    "ARROW_DOWN",
    "ARROW_DOWN_LEFT",
    "ARROW_DOWN_RIGHT",
    "ARROW_LEFT",
    "ARROW_RIGHT",
    "ARROW_UP",
    "ARROW_UP_LEFT",
    "ARROW_UP_RIGHT",
    "CARET_DOWN",
    "CARET_UP",
    "CHECKMARK",
    "CIRCLE",
    "FACE_DOWN",
    "FACE_FLAT",
    "FACE_UP",
    "FLAG",
    "MINUS",
    "ONE_BAR",
    "PLUS",
    "SQUARE",
    "THREE_BAR",
    "THUMBS_DOWN",
    "THUMBS_UP",
    "TRIANGLE",
    "TWO_BAR",
    "X",
]
```
## IdentityStoreType

```python
# IdentityStoreType usage example

from types_aiobotocore_quicksight.literals import IdentityStoreType

def get_value() -> IdentityStoreType:
    return "QUICKSIGHT"
```

```python
# IdentityStoreType definition

IdentityStoreType = Literal[
    "QUICKSIGHT",
]
```
## IdentityTypeType

```python
# IdentityTypeType usage example

from types_aiobotocore_quicksight.literals import IdentityTypeType

def get_value() -> IdentityTypeType:
    return "IAM"
```

```python
# IdentityTypeType definition

IdentityTypeType = Literal[
    "IAM",
    "IAM_IDENTITY_CENTER",
    "QUICKSIGHT",
]
```
## IngestionErrorTypeType

```python
# IngestionErrorTypeType usage example

from types_aiobotocore_quicksight.literals import IngestionErrorTypeType

def get_value() -> IngestionErrorTypeType:
    return "ACCOUNT_CAPACITY_LIMIT_EXCEEDED"
```

```python
# IngestionErrorTypeType definition

IngestionErrorTypeType = Literal[
    "ACCOUNT_CAPACITY_LIMIT_EXCEEDED",
    "CONNECTION_FAILURE",
    "CURSOR_NOT_ENABLED",
    "CUSTOMER_ERROR",
    "DATA_SET_DELETED",
    "DATA_SET_NOT_SPICE",
    "DATA_SET_SIZE_LIMIT_EXCEEDED",
    "DATA_SOURCE_AUTH_FAILED",
    "DATA_SOURCE_CONNECTION_FAILED",
    "DATA_SOURCE_NOT_FOUND",
    "DATA_TOLERANCE_EXCEPTION",
    "DUPLICATE_COLUMN_NAMES_FOUND",
    "ELASTICSEARCH_CURSOR_NOT_ENABLED",
    "FAILURE_TO_ASSUME_ROLE",
    "FAILURE_TO_PROCESS_JSON_FILE",
    "IAM_ROLE_NOT_AVAILABLE",
    "INGESTION_CANCELED",
    "INGESTION_SUPERSEDED",
    "INTERNAL_SERVICE_ERROR",
    "INVALID_DATA_SOURCE_CONFIG",
    "INVALID_DATAPREP_SYNTAX",
    "INVALID_DATE_FORMAT",
    "IOT_DATA_SET_FILE_EMPTY",
    "IOT_FILE_NOT_FOUND",
    "OAUTH_TOKEN_FAILURE",
    "PASSWORD_AUTHENTICATION_FAILURE",
    "PERMISSION_DENIED",
    "PERMISSION_NOT_FOUND",
    "QUERY_TIMEOUT",
    "REFRESH_SUPPRESSED_BY_EDIT",
    "ROW_SIZE_LIMIT_EXCEEDED",
    "S3_FILE_INACCESSIBLE",
    "S3_MANIFEST_ERROR",
    "S3_UPLOADED_FILE_DELETED",
    "SOURCE_API_LIMIT_EXCEEDED_FAILURE",
    "SOURCE_RESOURCE_LIMIT_EXCEEDED",
    "SPICE_TABLE_NOT_FOUND",
    "SQL_EXCEPTION",
    "SQL_INVALID_PARAMETER_VALUE",
    "SQL_NUMERIC_OVERFLOW",
    "SQL_SCHEMA_MISMATCH_ERROR",
    "SQL_TABLE_NOT_FOUND",
    "SSL_CERTIFICATE_VALIDATION_FAILURE",
    "UNRESOLVABLE_HOST",
    "UNROUTABLE_HOST",
]
```
## IngestionRequestSourceType

```python
# IngestionRequestSourceType usage example

from types_aiobotocore_quicksight.literals import IngestionRequestSourceType

def get_value() -> IngestionRequestSourceType:
    return "MANUAL"
```

```python
# IngestionRequestSourceType definition

IngestionRequestSourceType = Literal[
    "MANUAL",
    "SCHEDULED",
]
```
## IngestionRequestTypeType

```python
# IngestionRequestTypeType usage example

from types_aiobotocore_quicksight.literals import IngestionRequestTypeType

def get_value() -> IngestionRequestTypeType:
    return "EDIT"
```

```python
# IngestionRequestTypeType definition

IngestionRequestTypeType = Literal[
    "EDIT",
    "FULL_REFRESH",
    "INCREMENTAL_REFRESH",
    "INITIAL_INGESTION",
]
```
## IngestionStatusType

```python
# IngestionStatusType usage example

from types_aiobotocore_quicksight.literals import IngestionStatusType

def get_value() -> IngestionStatusType:
    return "CANCELLED"
```

```python
# IngestionStatusType definition

IngestionStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "INITIALIZED",
    "QUEUED",
    "RUNNING",
]
```
## IngestionTypeType

```python
# IngestionTypeType usage example

from types_aiobotocore_quicksight.literals import IngestionTypeType

def get_value() -> IngestionTypeType:
    return "FULL_REFRESH"
```

```python
# IngestionTypeType definition

IngestionTypeType = Literal[
    "FULL_REFRESH",
    "INCREMENTAL_REFRESH",
]
```
## InputColumnDataTypeType

```python
# InputColumnDataTypeType usage example

from types_aiobotocore_quicksight.literals import InputColumnDataTypeType

def get_value() -> InputColumnDataTypeType:
    return "BIT"
```

```python
# InputColumnDataTypeType definition

InputColumnDataTypeType = Literal[
    "BIT",
    "BOOLEAN",
    "DATETIME",
    "DECIMAL",
    "INTEGER",
    "JSON",
    "STRING",
]
```
## JoinTypeType

```python
# JoinTypeType usage example

from types_aiobotocore_quicksight.literals import JoinTypeType

def get_value() -> JoinTypeType:
    return "INNER"
```

```python
# JoinTypeType definition

JoinTypeType = Literal[
    "INNER",
    "LEFT",
    "OUTER",
    "RIGHT",
]
```
## LayoutElementTypeType

```python
# LayoutElementTypeType usage example

from types_aiobotocore_quicksight.literals import LayoutElementTypeType

def get_value() -> LayoutElementTypeType:
    return "FILTER_CONTROL"
```

```python
# LayoutElementTypeType definition

LayoutElementTypeType = Literal[
    "FILTER_CONTROL",
    "PARAMETER_CONTROL",
    "TEXT_BOX",
    "VISUAL",
]
```
## LegendPositionType

```python
# LegendPositionType usage example

from types_aiobotocore_quicksight.literals import LegendPositionType

def get_value() -> LegendPositionType:
    return "AUTO"
```

```python
# LegendPositionType definition

LegendPositionType = Literal[
    "AUTO",
    "BOTTOM",
    "RIGHT",
    "TOP",
]
```
## LineChartLineStyleType

```python
# LineChartLineStyleType usage example

from types_aiobotocore_quicksight.literals import LineChartLineStyleType

def get_value() -> LineChartLineStyleType:
    return "DASHED"
```

```python
# LineChartLineStyleType definition

LineChartLineStyleType = Literal[
    "DASHED",
    "DOTTED",
    "SOLID",
]
```
## LineChartMarkerShapeType

```python
# LineChartMarkerShapeType usage example

from types_aiobotocore_quicksight.literals import LineChartMarkerShapeType

def get_value() -> LineChartMarkerShapeType:
    return "CIRCLE"
```

```python
# LineChartMarkerShapeType definition

LineChartMarkerShapeType = Literal[
    "CIRCLE",
    "DIAMOND",
    "ROUNDED_SQUARE",
    "SQUARE",
    "TRIANGLE",
]
```
## LineChartTypeType

```python
# LineChartTypeType usage example

from types_aiobotocore_quicksight.literals import LineChartTypeType

def get_value() -> LineChartTypeType:
    return "AREA"
```

```python
# LineChartTypeType definition

LineChartTypeType = Literal[
    "AREA",
    "LINE",
    "STACKED_AREA",
]
```
## LineInterpolationType

```python
# LineInterpolationType usage example

from types_aiobotocore_quicksight.literals import LineInterpolationType

def get_value() -> LineInterpolationType:
    return "LINEAR"
```

```python
# LineInterpolationType definition

LineInterpolationType = Literal[
    "LINEAR",
    "SMOOTH",
    "STEPPED",
]
```
## ListAnalysesPaginatorName

```python
# ListAnalysesPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListAnalysesPaginatorName

def get_value() -> ListAnalysesPaginatorName:
    return "list_analyses"
```

```python
# ListAnalysesPaginatorName definition

ListAnalysesPaginatorName = Literal[
    "list_analyses",
]
```
## ListAssetBundleExportJobsPaginatorName

```python
# ListAssetBundleExportJobsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListAssetBundleExportJobsPaginatorName

def get_value() -> ListAssetBundleExportJobsPaginatorName:
    return "list_asset_bundle_export_jobs"
```

```python
# ListAssetBundleExportJobsPaginatorName definition

ListAssetBundleExportJobsPaginatorName = Literal[
    "list_asset_bundle_export_jobs",
]
```
## ListAssetBundleImportJobsPaginatorName

```python
# ListAssetBundleImportJobsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListAssetBundleImportJobsPaginatorName

def get_value() -> ListAssetBundleImportJobsPaginatorName:
    return "list_asset_bundle_import_jobs"
```

```python
# ListAssetBundleImportJobsPaginatorName definition

ListAssetBundleImportJobsPaginatorName = Literal[
    "list_asset_bundle_import_jobs",
]
```
## ListDashboardVersionsPaginatorName

```python
# ListDashboardVersionsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListDashboardVersionsPaginatorName

def get_value() -> ListDashboardVersionsPaginatorName:
    return "list_dashboard_versions"
```

```python
# ListDashboardVersionsPaginatorName definition

ListDashboardVersionsPaginatorName = Literal[
    "list_dashboard_versions",
]
```
## ListDashboardsPaginatorName

```python
# ListDashboardsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListDashboardsPaginatorName

def get_value() -> ListDashboardsPaginatorName:
    return "list_dashboards"
```

```python
# ListDashboardsPaginatorName definition

ListDashboardsPaginatorName = Literal[
    "list_dashboards",
]
```
## ListDataSetsPaginatorName

```python
# ListDataSetsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListDataSetsPaginatorName

def get_value() -> ListDataSetsPaginatorName:
    return "list_data_sets"
```

```python
# ListDataSetsPaginatorName definition

ListDataSetsPaginatorName = Literal[
    "list_data_sets",
]
```
## ListDataSourcesPaginatorName

```python
# ListDataSourcesPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListDataSourcesPaginatorName

def get_value() -> ListDataSourcesPaginatorName:
    return "list_data_sources"
```

```python
# ListDataSourcesPaginatorName definition

ListDataSourcesPaginatorName = Literal[
    "list_data_sources",
]
```
## ListGroupMembershipsPaginatorName

```python
# ListGroupMembershipsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListGroupMembershipsPaginatorName

def get_value() -> ListGroupMembershipsPaginatorName:
    return "list_group_memberships"
```

```python
# ListGroupMembershipsPaginatorName definition

ListGroupMembershipsPaginatorName = Literal[
    "list_group_memberships",
]
```
## ListGroupsPaginatorName

```python
# ListGroupsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListGroupsPaginatorName

def get_value() -> ListGroupsPaginatorName:
    return "list_groups"
```

```python
# ListGroupsPaginatorName definition

ListGroupsPaginatorName = Literal[
    "list_groups",
]
```
## ListIAMPolicyAssignmentsForUserPaginatorName

```python
# ListIAMPolicyAssignmentsForUserPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListIAMPolicyAssignmentsForUserPaginatorName

def get_value() -> ListIAMPolicyAssignmentsForUserPaginatorName:
    return "list_iam_policy_assignments_for_user"
```

```python
# ListIAMPolicyAssignmentsForUserPaginatorName definition

ListIAMPolicyAssignmentsForUserPaginatorName = Literal[
    "list_iam_policy_assignments_for_user",
]
```
## ListIAMPolicyAssignmentsPaginatorName

```python
# ListIAMPolicyAssignmentsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListIAMPolicyAssignmentsPaginatorName

def get_value() -> ListIAMPolicyAssignmentsPaginatorName:
    return "list_iam_policy_assignments"
```

```python
# ListIAMPolicyAssignmentsPaginatorName definition

ListIAMPolicyAssignmentsPaginatorName = Literal[
    "list_iam_policy_assignments",
]
```
## ListIngestionsPaginatorName

```python
# ListIngestionsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListIngestionsPaginatorName

def get_value() -> ListIngestionsPaginatorName:
    return "list_ingestions"
```

```python
# ListIngestionsPaginatorName definition

ListIngestionsPaginatorName = Literal[
    "list_ingestions",
]
```
## ListNamespacesPaginatorName

```python
# ListNamespacesPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListNamespacesPaginatorName

def get_value() -> ListNamespacesPaginatorName:
    return "list_namespaces"
```

```python
# ListNamespacesPaginatorName definition

ListNamespacesPaginatorName = Literal[
    "list_namespaces",
]
```
## ListTemplateAliasesPaginatorName

```python
# ListTemplateAliasesPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListTemplateAliasesPaginatorName

def get_value() -> ListTemplateAliasesPaginatorName:
    return "list_template_aliases"
```

```python
# ListTemplateAliasesPaginatorName definition

ListTemplateAliasesPaginatorName = Literal[
    "list_template_aliases",
]
```
## ListTemplateVersionsPaginatorName

```python
# ListTemplateVersionsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListTemplateVersionsPaginatorName

def get_value() -> ListTemplateVersionsPaginatorName:
    return "list_template_versions"
```

```python
# ListTemplateVersionsPaginatorName definition

ListTemplateVersionsPaginatorName = Literal[
    "list_template_versions",
]
```
## ListTemplatesPaginatorName

```python
# ListTemplatesPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListTemplatesPaginatorName

def get_value() -> ListTemplatesPaginatorName:
    return "list_templates"
```

```python
# ListTemplatesPaginatorName definition

ListTemplatesPaginatorName = Literal[
    "list_templates",
]
```
## ListThemeVersionsPaginatorName

```python
# ListThemeVersionsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListThemeVersionsPaginatorName

def get_value() -> ListThemeVersionsPaginatorName:
    return "list_theme_versions"
```

```python
# ListThemeVersionsPaginatorName definition

ListThemeVersionsPaginatorName = Literal[
    "list_theme_versions",
]
```
## ListThemesPaginatorName

```python
# ListThemesPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListThemesPaginatorName

def get_value() -> ListThemesPaginatorName:
    return "list_themes"
```

```python
# ListThemesPaginatorName definition

ListThemesPaginatorName = Literal[
    "list_themes",
]
```
## ListUserGroupsPaginatorName

```python
# ListUserGroupsPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListUserGroupsPaginatorName

def get_value() -> ListUserGroupsPaginatorName:
    return "list_user_groups"
```

```python
# ListUserGroupsPaginatorName definition

ListUserGroupsPaginatorName = Literal[
    "list_user_groups",
]
```
## ListUsersPaginatorName

```python
# ListUsersPaginatorName usage example

from types_aiobotocore_quicksight.literals import ListUsersPaginatorName

def get_value() -> ListUsersPaginatorName:
    return "list_users"
```

```python
# ListUsersPaginatorName definition

ListUsersPaginatorName = Literal[
    "list_users",
]
```
## LookbackWindowSizeUnitType

```python
# LookbackWindowSizeUnitType usage example

from types_aiobotocore_quicksight.literals import LookbackWindowSizeUnitType

def get_value() -> LookbackWindowSizeUnitType:
    return "DAY"
```

```python
# LookbackWindowSizeUnitType definition

LookbackWindowSizeUnitType = Literal[
    "DAY",
    "HOUR",
    "WEEK",
]
```
## MapZoomModeType

```python
# MapZoomModeType usage example

from types_aiobotocore_quicksight.literals import MapZoomModeType

def get_value() -> MapZoomModeType:
    return "AUTO"
```

```python
# MapZoomModeType definition

MapZoomModeType = Literal[
    "AUTO",
    "MANUAL",
]
```
## MaximumMinimumComputationTypeType

```python
# MaximumMinimumComputationTypeType usage example

from types_aiobotocore_quicksight.literals import MaximumMinimumComputationTypeType

def get_value() -> MaximumMinimumComputationTypeType:
    return "MAXIMUM"
```

```python
# MaximumMinimumComputationTypeType definition

MaximumMinimumComputationTypeType = Literal[
    "MAXIMUM",
    "MINIMUM",
]
```
## MemberTypeType

```python
# MemberTypeType usage example

from types_aiobotocore_quicksight.literals import MemberTypeType

def get_value() -> MemberTypeType:
    return "ANALYSIS"
```

```python
# MemberTypeType definition

MemberTypeType = Literal[
    "ANALYSIS",
    "DASHBOARD",
    "DATASET",
]
```
## MissingDataTreatmentOptionType

```python
# MissingDataTreatmentOptionType usage example

from types_aiobotocore_quicksight.literals import MissingDataTreatmentOptionType

def get_value() -> MissingDataTreatmentOptionType:
    return "INTERPOLATE"
```

```python
# MissingDataTreatmentOptionType definition

MissingDataTreatmentOptionType = Literal[
    "INTERPOLATE",
    "SHOW_AS_BLANK",
    "SHOW_AS_ZERO",
]
```
## NamedEntityAggTypeType

```python
# NamedEntityAggTypeType usage example

from types_aiobotocore_quicksight.literals import NamedEntityAggTypeType

def get_value() -> NamedEntityAggTypeType:
    return "AVERAGE"
```

```python
# NamedEntityAggTypeType definition

NamedEntityAggTypeType = Literal[
    "AVERAGE",
    "COUNT",
    "CUSTOM",
    "DISTINCT_COUNT",
    "MAX",
    "MEDIAN",
    "MIN",
    "PERCENTILE",
    "STDEV",
    "STDEVP",
    "SUM",
    "VAR",
    "VARP",
]
```
## NamedFilterAggTypeType

```python
# NamedFilterAggTypeType usage example

from types_aiobotocore_quicksight.literals import NamedFilterAggTypeType

def get_value() -> NamedFilterAggTypeType:
    return "AVERAGE"
```

```python
# NamedFilterAggTypeType definition

NamedFilterAggTypeType = Literal[
    "AVERAGE",
    "COUNT",
    "DISTINCT_COUNT",
    "MAX",
    "MEDIAN",
    "MIN",
    "NO_AGGREGATION",
    "STDEV",
    "STDEVP",
    "SUM",
    "VAR",
    "VARP",
]
```
## NamedFilterTypeType

```python
# NamedFilterTypeType usage example

from types_aiobotocore_quicksight.literals import NamedFilterTypeType

def get_value() -> NamedFilterTypeType:
    return "CATEGORY_FILTER"
```

```python
# NamedFilterTypeType definition

NamedFilterTypeType = Literal[
    "CATEGORY_FILTER",
    "DATE_RANGE_FILTER",
    "NUMERIC_EQUALITY_FILTER",
    "NUMERIC_RANGE_FILTER",
    "RELATIVE_DATE_FILTER",
]
```
## NamespaceErrorTypeType

```python
# NamespaceErrorTypeType usage example

from types_aiobotocore_quicksight.literals import NamespaceErrorTypeType

def get_value() -> NamespaceErrorTypeType:
    return "INTERNAL_SERVICE_ERROR"
```

```python
# NamespaceErrorTypeType definition

NamespaceErrorTypeType = Literal[
    "INTERNAL_SERVICE_ERROR",
    "PERMISSION_DENIED",
]
```
## NamespaceStatusType

```python
# NamespaceStatusType usage example

from types_aiobotocore_quicksight.literals import NamespaceStatusType

def get_value() -> NamespaceStatusType:
    return "CREATED"
```

```python
# NamespaceStatusType definition

NamespaceStatusType = Literal[
    "CREATED",
    "CREATING",
    "DELETING",
    "NON_RETRYABLE_FAILURE",
    "RETRYABLE_FAILURE",
]
```
## NegativeValueDisplayModeType

```python
# NegativeValueDisplayModeType usage example

from types_aiobotocore_quicksight.literals import NegativeValueDisplayModeType

def get_value() -> NegativeValueDisplayModeType:
    return "NEGATIVE"
```

```python
# NegativeValueDisplayModeType definition

NegativeValueDisplayModeType = Literal[
    "NEGATIVE",
    "POSITIVE",
]
```
## NetworkInterfaceStatusType

```python
# NetworkInterfaceStatusType usage example

from types_aiobotocore_quicksight.literals import NetworkInterfaceStatusType

def get_value() -> NetworkInterfaceStatusType:
    return "ATTACHMENT_FAILED_ROLLBACK_FAILED"
```

```python
# NetworkInterfaceStatusType definition

NetworkInterfaceStatusType = Literal[
    "ATTACHMENT_FAILED_ROLLBACK_FAILED",
    "AVAILABLE",
    "CREATING",
    "CREATION_FAILED",
    "DELETED",
    "DELETING",
    "DELETION_FAILED",
    "DELETION_SCHEDULED",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## NumberScaleType

```python
# NumberScaleType usage example

from types_aiobotocore_quicksight.literals import NumberScaleType

def get_value() -> NumberScaleType:
    return "AUTO"
```

```python
# NumberScaleType definition

NumberScaleType = Literal[
    "AUTO",
    "BILLIONS",
    "MILLIONS",
    "NONE",
    "THOUSANDS",
    "TRILLIONS",
]
```
## NumericEqualityMatchOperatorType

```python
# NumericEqualityMatchOperatorType usage example

from types_aiobotocore_quicksight.literals import NumericEqualityMatchOperatorType

def get_value() -> NumericEqualityMatchOperatorType:
    return "DOES_NOT_EQUAL"
```

```python
# NumericEqualityMatchOperatorType definition

NumericEqualityMatchOperatorType = Literal[
    "DOES_NOT_EQUAL",
    "EQUALS",
]
```
## NumericFilterSelectAllOptionsType

```python
# NumericFilterSelectAllOptionsType usage example

from types_aiobotocore_quicksight.literals import NumericFilterSelectAllOptionsType

def get_value() -> NumericFilterSelectAllOptionsType:
    return "FILTER_ALL_VALUES"
```

```python
# NumericFilterSelectAllOptionsType definition

NumericFilterSelectAllOptionsType = Literal[
    "FILTER_ALL_VALUES",
]
```
## NumericSeparatorSymbolType

```python
# NumericSeparatorSymbolType usage example

from types_aiobotocore_quicksight.literals import NumericSeparatorSymbolType

def get_value() -> NumericSeparatorSymbolType:
    return "COMMA"
```

```python
# NumericSeparatorSymbolType definition

NumericSeparatorSymbolType = Literal[
    "COMMA",
    "DOT",
    "SPACE",
]
```
## OtherCategoriesType

```python
# OtherCategoriesType usage example

from types_aiobotocore_quicksight.literals import OtherCategoriesType

def get_value() -> OtherCategoriesType:
    return "EXCLUDE"
```

```python
# OtherCategoriesType definition

OtherCategoriesType = Literal[
    "EXCLUDE",
    "INCLUDE",
]
```
## PanelBorderStyleType

```python
# PanelBorderStyleType usage example

from types_aiobotocore_quicksight.literals import PanelBorderStyleType

def get_value() -> PanelBorderStyleType:
    return "DASHED"
```

```python
# PanelBorderStyleType definition

PanelBorderStyleType = Literal[
    "DASHED",
    "DOTTED",
    "SOLID",
]
```
## PaperOrientationType

```python
# PaperOrientationType usage example

from types_aiobotocore_quicksight.literals import PaperOrientationType

def get_value() -> PaperOrientationType:
    return "LANDSCAPE"
```

```python
# PaperOrientationType definition

PaperOrientationType = Literal[
    "LANDSCAPE",
    "PORTRAIT",
]
```
## PaperSizeType

```python
# PaperSizeType usage example

from types_aiobotocore_quicksight.literals import PaperSizeType

def get_value() -> PaperSizeType:
    return "A0"
```

```python
# PaperSizeType definition

PaperSizeType = Literal[
    "A0",
    "A1",
    "A2",
    "A3",
    "A4",
    "A5",
    "JIS_B4",
    "JIS_B5",
    "US_LEGAL",
    "US_LETTER",
    "US_TABLOID_LEDGER",
]
```
## ParameterValueTypeType

```python
# ParameterValueTypeType usage example

from types_aiobotocore_quicksight.literals import ParameterValueTypeType

def get_value() -> ParameterValueTypeType:
    return "MULTI_VALUED"
```

```python
# ParameterValueTypeType definition

ParameterValueTypeType = Literal[
    "MULTI_VALUED",
    "SINGLE_VALUED",
]
```
## PivotTableConditionalFormattingScopeRoleType

```python
# PivotTableConditionalFormattingScopeRoleType usage example

from types_aiobotocore_quicksight.literals import PivotTableConditionalFormattingScopeRoleType

def get_value() -> PivotTableConditionalFormattingScopeRoleType:
    return "FIELD"
```

```python
# PivotTableConditionalFormattingScopeRoleType definition

PivotTableConditionalFormattingScopeRoleType = Literal[
    "FIELD",
    "FIELD_TOTAL",
    "GRAND_TOTAL",
]
```
## PivotTableFieldCollapseStateType

```python
# PivotTableFieldCollapseStateType usage example

from types_aiobotocore_quicksight.literals import PivotTableFieldCollapseStateType

def get_value() -> PivotTableFieldCollapseStateType:
    return "COLLAPSED"
```

```python
# PivotTableFieldCollapseStateType definition

PivotTableFieldCollapseStateType = Literal[
    "COLLAPSED",
    "EXPANDED",
]
```
## PivotTableMetricPlacementType

```python
# PivotTableMetricPlacementType usage example

from types_aiobotocore_quicksight.literals import PivotTableMetricPlacementType

def get_value() -> PivotTableMetricPlacementType:
    return "COLUMN"
```

```python
# PivotTableMetricPlacementType definition

PivotTableMetricPlacementType = Literal[
    "COLUMN",
    "ROW",
]
```
## PivotTableRowsLayoutType

```python
# PivotTableRowsLayoutType usage example

from types_aiobotocore_quicksight.literals import PivotTableRowsLayoutType

def get_value() -> PivotTableRowsLayoutType:
    return "HIERARCHY"
```

```python
# PivotTableRowsLayoutType definition

PivotTableRowsLayoutType = Literal[
    "HIERARCHY",
    "TABULAR",
]
```
## PivotTableSubtotalLevelType

```python
# PivotTableSubtotalLevelType usage example

from types_aiobotocore_quicksight.literals import PivotTableSubtotalLevelType

def get_value() -> PivotTableSubtotalLevelType:
    return "ALL"
```

```python
# PivotTableSubtotalLevelType definition

PivotTableSubtotalLevelType = Literal[
    "ALL",
    "CUSTOM",
    "LAST",
]
```
## PrimaryValueDisplayTypeType

```python
# PrimaryValueDisplayTypeType usage example

from types_aiobotocore_quicksight.literals import PrimaryValueDisplayTypeType

def get_value() -> PrimaryValueDisplayTypeType:
    return "ACTUAL"
```

```python
# PrimaryValueDisplayTypeType definition

PrimaryValueDisplayTypeType = Literal[
    "ACTUAL",
    "COMPARISON",
    "HIDDEN",
]
```
## PropertyRoleType

```python
# PropertyRoleType usage example

from types_aiobotocore_quicksight.literals import PropertyRoleType

def get_value() -> PropertyRoleType:
    return "ID"
```

```python
# PropertyRoleType definition

PropertyRoleType = Literal[
    "ID",
    "PRIMARY",
]
```
## PropertyUsageType

```python
# PropertyUsageType usage example

from types_aiobotocore_quicksight.literals import PropertyUsageType

def get_value() -> PropertyUsageType:
    return "DIMENSION"
```

```python
# PropertyUsageType definition

PropertyUsageType = Literal[
    "DIMENSION",
    "INHERIT",
    "MEASURE",
]
```
## RadarChartAxesRangeScaleType

```python
# RadarChartAxesRangeScaleType usage example

from types_aiobotocore_quicksight.literals import RadarChartAxesRangeScaleType

def get_value() -> RadarChartAxesRangeScaleType:
    return "AUTO"
```

```python
# RadarChartAxesRangeScaleType definition

RadarChartAxesRangeScaleType = Literal[
    "AUTO",
    "INDEPENDENT",
    "SHARED",
]
```
## RadarChartShapeType

```python
# RadarChartShapeType usage example

from types_aiobotocore_quicksight.literals import RadarChartShapeType

def get_value() -> RadarChartShapeType:
    return "CIRCLE"
```

```python
# RadarChartShapeType definition

RadarChartShapeType = Literal[
    "CIRCLE",
    "POLYGON",
]
```
## ReferenceLineLabelHorizontalPositionType

```python
# ReferenceLineLabelHorizontalPositionType usage example

from types_aiobotocore_quicksight.literals import ReferenceLineLabelHorizontalPositionType

def get_value() -> ReferenceLineLabelHorizontalPositionType:
    return "CENTER"
```

```python
# ReferenceLineLabelHorizontalPositionType definition

ReferenceLineLabelHorizontalPositionType = Literal[
    "CENTER",
    "LEFT",
    "RIGHT",
]
```
## ReferenceLineLabelVerticalPositionType

```python
# ReferenceLineLabelVerticalPositionType usage example

from types_aiobotocore_quicksight.literals import ReferenceLineLabelVerticalPositionType

def get_value() -> ReferenceLineLabelVerticalPositionType:
    return "ABOVE"
```

```python
# ReferenceLineLabelVerticalPositionType definition

ReferenceLineLabelVerticalPositionType = Literal[
    "ABOVE",
    "BELOW",
]
```
## ReferenceLinePatternTypeType

```python
# ReferenceLinePatternTypeType usage example

from types_aiobotocore_quicksight.literals import ReferenceLinePatternTypeType

def get_value() -> ReferenceLinePatternTypeType:
    return "DASHED"
```

```python
# ReferenceLinePatternTypeType definition

ReferenceLinePatternTypeType = Literal[
    "DASHED",
    "DOTTED",
    "SOLID",
]
```
## ReferenceLineValueLabelRelativePositionType

```python
# ReferenceLineValueLabelRelativePositionType usage example

from types_aiobotocore_quicksight.literals import ReferenceLineValueLabelRelativePositionType

def get_value() -> ReferenceLineValueLabelRelativePositionType:
    return "AFTER_CUSTOM_LABEL"
```

```python
# ReferenceLineValueLabelRelativePositionType definition

ReferenceLineValueLabelRelativePositionType = Literal[
    "AFTER_CUSTOM_LABEL",
    "BEFORE_CUSTOM_LABEL",
]
```
## RefreshIntervalType

```python
# RefreshIntervalType usage example

from types_aiobotocore_quicksight.literals import RefreshIntervalType

def get_value() -> RefreshIntervalType:
    return "DAILY"
```

```python
# RefreshIntervalType definition

RefreshIntervalType = Literal[
    "DAILY",
    "HOURLY",
    "MINUTE15",
    "MINUTE30",
    "MONTHLY",
    "WEEKLY",
]
```
## RelativeDateTypeType

```python
# RelativeDateTypeType usage example

from types_aiobotocore_quicksight.literals import RelativeDateTypeType

def get_value() -> RelativeDateTypeType:
    return "LAST"
```

```python
# RelativeDateTypeType definition

RelativeDateTypeType = Literal[
    "LAST",
    "NEXT",
    "NOW",
    "PREVIOUS",
    "THIS",
]
```
## RelativeFontSizeType

```python
# RelativeFontSizeType usage example

from types_aiobotocore_quicksight.literals import RelativeFontSizeType

def get_value() -> RelativeFontSizeType:
    return "EXTRA_LARGE"
```

```python
# RelativeFontSizeType definition

RelativeFontSizeType = Literal[
    "EXTRA_LARGE",
    "EXTRA_SMALL",
    "LARGE",
    "MEDIUM",
    "SMALL",
]
```
## ResizeOptionType

```python
# ResizeOptionType usage example

from types_aiobotocore_quicksight.literals import ResizeOptionType

def get_value() -> ResizeOptionType:
    return "FIXED"
```

```python
# ResizeOptionType definition

ResizeOptionType = Literal[
    "FIXED",
    "RESPONSIVE",
]
```
## ResourceStatusType

```python
# ResourceStatusType usage example

from types_aiobotocore_quicksight.literals import ResourceStatusType

def get_value() -> ResourceStatusType:
    return "CREATION_FAILED"
```

```python
# ResourceStatusType definition

ResourceStatusType = Literal[
    "CREATION_FAILED",
    "CREATION_IN_PROGRESS",
    "CREATION_SUCCESSFUL",
    "DELETED",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
    "UPDATE_SUCCESSFUL",
]
```
## RowLevelPermissionFormatVersionType

```python
# RowLevelPermissionFormatVersionType usage example

from types_aiobotocore_quicksight.literals import RowLevelPermissionFormatVersionType

def get_value() -> RowLevelPermissionFormatVersionType:
    return "VERSION_1"
```

```python
# RowLevelPermissionFormatVersionType definition

RowLevelPermissionFormatVersionType = Literal[
    "VERSION_1",
    "VERSION_2",
]
```
## RowLevelPermissionPolicyType

```python
# RowLevelPermissionPolicyType usage example

from types_aiobotocore_quicksight.literals import RowLevelPermissionPolicyType

def get_value() -> RowLevelPermissionPolicyType:
    return "DENY_ACCESS"
```

```python
# RowLevelPermissionPolicyType definition

RowLevelPermissionPolicyType = Literal[
    "DENY_ACCESS",
    "GRANT_ACCESS",
]
```
## SearchAnalysesPaginatorName

```python
# SearchAnalysesPaginatorName usage example

from types_aiobotocore_quicksight.literals import SearchAnalysesPaginatorName

def get_value() -> SearchAnalysesPaginatorName:
    return "search_analyses"
```

```python
# SearchAnalysesPaginatorName definition

SearchAnalysesPaginatorName = Literal[
    "search_analyses",
]
```
## SearchDashboardsPaginatorName

```python
# SearchDashboardsPaginatorName usage example

from types_aiobotocore_quicksight.literals import SearchDashboardsPaginatorName

def get_value() -> SearchDashboardsPaginatorName:
    return "search_dashboards"
```

```python
# SearchDashboardsPaginatorName definition

SearchDashboardsPaginatorName = Literal[
    "search_dashboards",
]
```
## SearchDataSetsPaginatorName

```python
# SearchDataSetsPaginatorName usage example

from types_aiobotocore_quicksight.literals import SearchDataSetsPaginatorName

def get_value() -> SearchDataSetsPaginatorName:
    return "search_data_sets"
```

```python
# SearchDataSetsPaginatorName definition

SearchDataSetsPaginatorName = Literal[
    "search_data_sets",
]
```
## SearchDataSourcesPaginatorName

```python
# SearchDataSourcesPaginatorName usage example

from types_aiobotocore_quicksight.literals import SearchDataSourcesPaginatorName

def get_value() -> SearchDataSourcesPaginatorName:
    return "search_data_sources"
```

```python
# SearchDataSourcesPaginatorName definition

SearchDataSourcesPaginatorName = Literal[
    "search_data_sources",
]
```
## SearchGroupsPaginatorName

```python
# SearchGroupsPaginatorName usage example

from types_aiobotocore_quicksight.literals import SearchGroupsPaginatorName

def get_value() -> SearchGroupsPaginatorName:
    return "search_groups"
```

```python
# SearchGroupsPaginatorName definition

SearchGroupsPaginatorName = Literal[
    "search_groups",
]
```
## SectionPageBreakStatusType

```python
# SectionPageBreakStatusType usage example

from types_aiobotocore_quicksight.literals import SectionPageBreakStatusType

def get_value() -> SectionPageBreakStatusType:
    return "DISABLED"
```

```python
# SectionPageBreakStatusType definition

SectionPageBreakStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## SelectAllValueOptionsType

```python
# SelectAllValueOptionsType usage example

from types_aiobotocore_quicksight.literals import SelectAllValueOptionsType

def get_value() -> SelectAllValueOptionsType:
    return "ALL_VALUES"
```

```python
# SelectAllValueOptionsType definition

SelectAllValueOptionsType = Literal[
    "ALL_VALUES",
]
```
## SelectedFieldOptionsType

```python
# SelectedFieldOptionsType usage example

from types_aiobotocore_quicksight.literals import SelectedFieldOptionsType

def get_value() -> SelectedFieldOptionsType:
    return "ALL_FIELDS"
```

```python
# SelectedFieldOptionsType definition

SelectedFieldOptionsType = Literal[
    "ALL_FIELDS",
]
```
## SelectedTooltipTypeType

```python
# SelectedTooltipTypeType usage example

from types_aiobotocore_quicksight.literals import SelectedTooltipTypeType

def get_value() -> SelectedTooltipTypeType:
    return "BASIC"
```

```python
# SelectedTooltipTypeType definition

SelectedTooltipTypeType = Literal[
    "BASIC",
    "DETAILED",
]
```
## SheetContentTypeType

```python
# SheetContentTypeType usage example

from types_aiobotocore_quicksight.literals import SheetContentTypeType

def get_value() -> SheetContentTypeType:
    return "INTERACTIVE"
```

```python
# SheetContentTypeType definition

SheetContentTypeType = Literal[
    "INTERACTIVE",
    "PAGINATED",
]
```
## SheetControlDateTimePickerTypeType

```python
# SheetControlDateTimePickerTypeType usage example

from types_aiobotocore_quicksight.literals import SheetControlDateTimePickerTypeType

def get_value() -> SheetControlDateTimePickerTypeType:
    return "DATE_RANGE"
```

```python
# SheetControlDateTimePickerTypeType definition

SheetControlDateTimePickerTypeType = Literal[
    "DATE_RANGE",
    "SINGLE_VALUED",
]
```
## SheetControlListTypeType

```python
# SheetControlListTypeType usage example

from types_aiobotocore_quicksight.literals import SheetControlListTypeType

def get_value() -> SheetControlListTypeType:
    return "MULTI_SELECT"
```

```python
# SheetControlListTypeType definition

SheetControlListTypeType = Literal[
    "MULTI_SELECT",
    "SINGLE_SELECT",
]
```
## SheetControlSliderTypeType

```python
# SheetControlSliderTypeType usage example

from types_aiobotocore_quicksight.literals import SheetControlSliderTypeType

def get_value() -> SheetControlSliderTypeType:
    return "RANGE"
```

```python
# SheetControlSliderTypeType definition

SheetControlSliderTypeType = Literal[
    "RANGE",
    "SINGLE_POINT",
]
```
## SimpleAttributeAggregationFunctionType

```python
# SimpleAttributeAggregationFunctionType usage example

from types_aiobotocore_quicksight.literals import SimpleAttributeAggregationFunctionType

def get_value() -> SimpleAttributeAggregationFunctionType:
    return "UNIQUE_VALUE"
```

```python
# SimpleAttributeAggregationFunctionType definition

SimpleAttributeAggregationFunctionType = Literal[
    "UNIQUE_VALUE",
]
```
## SimpleNumericalAggregationFunctionType

```python
# SimpleNumericalAggregationFunctionType usage example

from types_aiobotocore_quicksight.literals import SimpleNumericalAggregationFunctionType

def get_value() -> SimpleNumericalAggregationFunctionType:
    return "AVERAGE"
```

```python
# SimpleNumericalAggregationFunctionType definition

SimpleNumericalAggregationFunctionType = Literal[
    "AVERAGE",
    "COUNT",
    "DISTINCT_COUNT",
    "MAX",
    "MEDIAN",
    "MIN",
    "STDEV",
    "STDEVP",
    "SUM",
    "VAR",
    "VARP",
]
```
## SmallMultiplesAxisPlacementType

```python
# SmallMultiplesAxisPlacementType usage example

from types_aiobotocore_quicksight.literals import SmallMultiplesAxisPlacementType

def get_value() -> SmallMultiplesAxisPlacementType:
    return "INSIDE"
```

```python
# SmallMultiplesAxisPlacementType definition

SmallMultiplesAxisPlacementType = Literal[
    "INSIDE",
    "OUTSIDE",
]
```
## SmallMultiplesAxisScaleType

```python
# SmallMultiplesAxisScaleType usage example

from types_aiobotocore_quicksight.literals import SmallMultiplesAxisScaleType

def get_value() -> SmallMultiplesAxisScaleType:
    return "INDEPENDENT"
```

```python
# SmallMultiplesAxisScaleType definition

SmallMultiplesAxisScaleType = Literal[
    "INDEPENDENT",
    "SHARED",
]
```
## SnapshotFileFormatTypeType

```python
# SnapshotFileFormatTypeType usage example

from types_aiobotocore_quicksight.literals import SnapshotFileFormatTypeType

def get_value() -> SnapshotFileFormatTypeType:
    return "CSV"
```

```python
# SnapshotFileFormatTypeType definition

SnapshotFileFormatTypeType = Literal[
    "CSV",
    "PDF",
]
```
## SnapshotFileSheetSelectionScopeType

```python
# SnapshotFileSheetSelectionScopeType usage example

from types_aiobotocore_quicksight.literals import SnapshotFileSheetSelectionScopeType

def get_value() -> SnapshotFileSheetSelectionScopeType:
    return "ALL_VISUALS"
```

```python
# SnapshotFileSheetSelectionScopeType definition

SnapshotFileSheetSelectionScopeType = Literal[
    "ALL_VISUALS",
    "SELECTED_VISUALS",
]
```
## SnapshotJobStatusType

```python
# SnapshotJobStatusType usage example

from types_aiobotocore_quicksight.literals import SnapshotJobStatusType

def get_value() -> SnapshotJobStatusType:
    return "COMPLETED"
```

```python
# SnapshotJobStatusType definition

SnapshotJobStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "QUEUED",
    "RUNNING",
]
```
## SortDirectionType

```python
# SortDirectionType usage example

from types_aiobotocore_quicksight.literals import SortDirectionType

def get_value() -> SortDirectionType:
    return "ASC"
```

```python
# SortDirectionType definition

SortDirectionType = Literal[
    "ASC",
    "DESC",
]
```
## SpecialValueType

```python
# SpecialValueType usage example

from types_aiobotocore_quicksight.literals import SpecialValueType

def get_value() -> SpecialValueType:
    return "EMPTY"
```

```python
# SpecialValueType definition

SpecialValueType = Literal[
    "EMPTY",
    "NULL",
    "OTHER",
]
```
## StatusType

```python
# StatusType usage example

from types_aiobotocore_quicksight.literals import StatusType

def get_value() -> StatusType:
    return "DISABLED"
```

```python
# StatusType definition

StatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## StyledCellTypeType

```python
# StyledCellTypeType usage example

from types_aiobotocore_quicksight.literals import StyledCellTypeType

def get_value() -> StyledCellTypeType:
    return "METRIC_HEADER"
```

```python
# StyledCellTypeType definition

StyledCellTypeType = Literal[
    "METRIC_HEADER",
    "TOTAL",
    "VALUE",
]
```
## TableBorderStyleType

```python
# TableBorderStyleType usage example

from types_aiobotocore_quicksight.literals import TableBorderStyleType

def get_value() -> TableBorderStyleType:
    return "NONE"
```

```python
# TableBorderStyleType definition

TableBorderStyleType = Literal[
    "NONE",
    "SOLID",
]
```
## TableCellImageScalingConfigurationType

```python
# TableCellImageScalingConfigurationType usage example

from types_aiobotocore_quicksight.literals import TableCellImageScalingConfigurationType

def get_value() -> TableCellImageScalingConfigurationType:
    return "DO_NOT_SCALE"
```

```python
# TableCellImageScalingConfigurationType definition

TableCellImageScalingConfigurationType = Literal[
    "DO_NOT_SCALE",
    "FIT_TO_CELL_HEIGHT",
    "FIT_TO_CELL_WIDTH",
]
```
## TableFieldIconSetTypeType

```python
# TableFieldIconSetTypeType usage example

from types_aiobotocore_quicksight.literals import TableFieldIconSetTypeType

def get_value() -> TableFieldIconSetTypeType:
    return "LINK"
```

```python
# TableFieldIconSetTypeType definition

TableFieldIconSetTypeType = Literal[
    "LINK",
]
```
## TableOrientationType

```python
# TableOrientationType usage example

from types_aiobotocore_quicksight.literals import TableOrientationType

def get_value() -> TableOrientationType:
    return "HORIZONTAL"
```

```python
# TableOrientationType definition

TableOrientationType = Literal[
    "HORIZONTAL",
    "VERTICAL",
]
```
## TableTotalsPlacementType

```python
# TableTotalsPlacementType usage example

from types_aiobotocore_quicksight.literals import TableTotalsPlacementType

def get_value() -> TableTotalsPlacementType:
    return "END"
```

```python
# TableTotalsPlacementType definition

TableTotalsPlacementType = Literal[
    "END",
    "START",
]
```
## TableTotalsScrollStatusType

```python
# TableTotalsScrollStatusType usage example

from types_aiobotocore_quicksight.literals import TableTotalsScrollStatusType

def get_value() -> TableTotalsScrollStatusType:
    return "PINNED"
```

```python
# TableTotalsScrollStatusType definition

TableTotalsScrollStatusType = Literal[
    "PINNED",
    "SCROLLED",
]
```
## TargetVisualOptionsType

```python
# TargetVisualOptionsType usage example

from types_aiobotocore_quicksight.literals import TargetVisualOptionsType

def get_value() -> TargetVisualOptionsType:
    return "ALL_VISUALS"
```

```python
# TargetVisualOptionsType definition

TargetVisualOptionsType = Literal[
    "ALL_VISUALS",
]
```
## TemplateErrorTypeType

```python
# TemplateErrorTypeType usage example

from types_aiobotocore_quicksight.literals import TemplateErrorTypeType

def get_value() -> TemplateErrorTypeType:
    return "ACCESS_DENIED"
```

```python
# TemplateErrorTypeType definition

TemplateErrorTypeType = Literal[
    "ACCESS_DENIED",
    "DATA_SET_NOT_FOUND",
    "INTERNAL_FAILURE",
    "SOURCE_NOT_FOUND",
]
```
## TextQualifierType

```python
# TextQualifierType usage example

from types_aiobotocore_quicksight.literals import TextQualifierType

def get_value() -> TextQualifierType:
    return "DOUBLE_QUOTE"
```

```python
# TextQualifierType definition

TextQualifierType = Literal[
    "DOUBLE_QUOTE",
    "SINGLE_QUOTE",
]
```
## TextWrapType

```python
# TextWrapType usage example

from types_aiobotocore_quicksight.literals import TextWrapType

def get_value() -> TextWrapType:
    return "NONE"
```

```python
# TextWrapType definition

TextWrapType = Literal[
    "NONE",
    "WRAP",
]
```
## ThemeErrorTypeType

```python
# ThemeErrorTypeType usage example

from types_aiobotocore_quicksight.literals import ThemeErrorTypeType

def get_value() -> ThemeErrorTypeType:
    return "INTERNAL_FAILURE"
```

```python
# ThemeErrorTypeType definition

ThemeErrorTypeType = Literal[
    "INTERNAL_FAILURE",
]
```
## ThemeTypeType

```python
# ThemeTypeType usage example

from types_aiobotocore_quicksight.literals import ThemeTypeType

def get_value() -> ThemeTypeType:
    return "ALL"
```

```python
# ThemeTypeType definition

ThemeTypeType = Literal[
    "ALL",
    "CUSTOM",
    "QUICKSIGHT",
]
```
## TimeGranularityType

```python
# TimeGranularityType usage example

from types_aiobotocore_quicksight.literals import TimeGranularityType

def get_value() -> TimeGranularityType:
    return "DAY"
```

```python
# TimeGranularityType definition

TimeGranularityType = Literal[
    "DAY",
    "HOUR",
    "MILLISECOND",
    "MINUTE",
    "MONTH",
    "QUARTER",
    "SECOND",
    "WEEK",
    "YEAR",
]
```
## TooltipTitleTypeType

```python
# TooltipTitleTypeType usage example

from types_aiobotocore_quicksight.literals import TooltipTitleTypeType

def get_value() -> TooltipTitleTypeType:
    return "NONE"
```

```python
# TooltipTitleTypeType definition

TooltipTitleTypeType = Literal[
    "NONE",
    "PRIMARY_VALUE",
]
```
## TopBottomComputationTypeType

```python
# TopBottomComputationTypeType usage example

from types_aiobotocore_quicksight.literals import TopBottomComputationTypeType

def get_value() -> TopBottomComputationTypeType:
    return "BOTTOM"
```

```python
# TopBottomComputationTypeType definition

TopBottomComputationTypeType = Literal[
    "BOTTOM",
    "TOP",
]
```
## TopBottomSortOrderType

```python
# TopBottomSortOrderType usage example

from types_aiobotocore_quicksight.literals import TopBottomSortOrderType

def get_value() -> TopBottomSortOrderType:
    return "ABSOLUTE_DIFFERENCE"
```

```python
# TopBottomSortOrderType definition

TopBottomSortOrderType = Literal[
    "ABSOLUTE_DIFFERENCE",
    "PERCENT_DIFFERENCE",
]
```
## TopicNumericSeparatorSymbolType

```python
# TopicNumericSeparatorSymbolType usage example

from types_aiobotocore_quicksight.literals import TopicNumericSeparatorSymbolType

def get_value() -> TopicNumericSeparatorSymbolType:
    return "COMMA"
```

```python
# TopicNumericSeparatorSymbolType definition

TopicNumericSeparatorSymbolType = Literal[
    "COMMA",
    "DOT",
]
```
## TopicRefreshStatusType

```python
# TopicRefreshStatusType usage example

from types_aiobotocore_quicksight.literals import TopicRefreshStatusType

def get_value() -> TopicRefreshStatusType:
    return "CANCELLED"
```

```python
# TopicRefreshStatusType definition

TopicRefreshStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "INITIALIZED",
    "RUNNING",
]
```
## TopicRelativeDateFilterFunctionType

```python
# TopicRelativeDateFilterFunctionType usage example

from types_aiobotocore_quicksight.literals import TopicRelativeDateFilterFunctionType

def get_value() -> TopicRelativeDateFilterFunctionType:
    return "LAST"
```

```python
# TopicRelativeDateFilterFunctionType definition

TopicRelativeDateFilterFunctionType = Literal[
    "LAST",
    "NEXT",
    "NOW",
    "PREVIOUS",
    "THIS",
]
```
## TopicScheduleTypeType

```python
# TopicScheduleTypeType usage example

from types_aiobotocore_quicksight.literals import TopicScheduleTypeType

def get_value() -> TopicScheduleTypeType:
    return "DAILY"
```

```python
# TopicScheduleTypeType definition

TopicScheduleTypeType = Literal[
    "DAILY",
    "HOURLY",
    "MONTHLY",
    "WEEKLY",
]
```
## TopicTimeGranularityType

```python
# TopicTimeGranularityType usage example

from types_aiobotocore_quicksight.literals import TopicTimeGranularityType

def get_value() -> TopicTimeGranularityType:
    return "DAY"
```

```python
# TopicTimeGranularityType definition

TopicTimeGranularityType = Literal[
    "DAY",
    "HOUR",
    "MINUTE",
    "MONTH",
    "QUARTER",
    "SECOND",
    "WEEK",
    "YEAR",
]
```
## URLTargetConfigurationType

```python
# URLTargetConfigurationType usage example

from types_aiobotocore_quicksight.literals import URLTargetConfigurationType

def get_value() -> URLTargetConfigurationType:
    return "NEW_TAB"
```

```python
# URLTargetConfigurationType definition

URLTargetConfigurationType = Literal[
    "NEW_TAB",
    "NEW_WINDOW",
    "SAME_TAB",
]
```
## UndefinedSpecifiedValueTypeType

```python
# UndefinedSpecifiedValueTypeType usage example

from types_aiobotocore_quicksight.literals import UndefinedSpecifiedValueTypeType

def get_value() -> UndefinedSpecifiedValueTypeType:
    return "LEAST"
```

```python
# UndefinedSpecifiedValueTypeType definition

UndefinedSpecifiedValueTypeType = Literal[
    "LEAST",
    "MOST",
]
```
## UserRoleType

```python
# UserRoleType usage example

from types_aiobotocore_quicksight.literals import UserRoleType

def get_value() -> UserRoleType:
    return "ADMIN"
```

```python
# UserRoleType definition

UserRoleType = Literal[
    "ADMIN",
    "AUTHOR",
    "READER",
    "RESTRICTED_AUTHOR",
    "RESTRICTED_READER",
]
```
## VPCConnectionAvailabilityStatusType

```python
# VPCConnectionAvailabilityStatusType usage example

from types_aiobotocore_quicksight.literals import VPCConnectionAvailabilityStatusType

def get_value() -> VPCConnectionAvailabilityStatusType:
    return "AVAILABLE"
```

```python
# VPCConnectionAvailabilityStatusType definition

VPCConnectionAvailabilityStatusType = Literal[
    "AVAILABLE",
    "PARTIALLY_AVAILABLE",
    "UNAVAILABLE",
]
```
## VPCConnectionResourceStatusType

```python
# VPCConnectionResourceStatusType usage example

from types_aiobotocore_quicksight.literals import VPCConnectionResourceStatusType

def get_value() -> VPCConnectionResourceStatusType:
    return "CREATION_FAILED"
```

```python
# VPCConnectionResourceStatusType definition

VPCConnectionResourceStatusType = Literal[
    "CREATION_FAILED",
    "CREATION_IN_PROGRESS",
    "CREATION_SUCCESSFUL",
    "DELETED",
    "DELETION_FAILED",
    "DELETION_IN_PROGRESS",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
    "UPDATE_SUCCESSFUL",
]
```
## ValueWhenUnsetOptionType

```python
# ValueWhenUnsetOptionType usage example

from types_aiobotocore_quicksight.literals import ValueWhenUnsetOptionType

def get_value() -> ValueWhenUnsetOptionType:
    return "NULL"
```

```python
# ValueWhenUnsetOptionType definition

ValueWhenUnsetOptionType = Literal[
    "NULL",
    "RECOMMENDED_VALUE",
]
```
## VerticalTextAlignmentType

```python
# VerticalTextAlignmentType usage example

from types_aiobotocore_quicksight.literals import VerticalTextAlignmentType

def get_value() -> VerticalTextAlignmentType:
    return "AUTO"
```

```python
# VerticalTextAlignmentType definition

VerticalTextAlignmentType = Literal[
    "AUTO",
    "BOTTOM",
    "MIDDLE",
    "TOP",
]
```
## VisibilityType

```python
# VisibilityType usage example

from types_aiobotocore_quicksight.literals import VisibilityType

def get_value() -> VisibilityType:
    return "HIDDEN"
```

```python
# VisibilityType definition

VisibilityType = Literal[
    "HIDDEN",
    "VISIBLE",
]
```
## VisualCustomActionTriggerType

```python
# VisualCustomActionTriggerType usage example

from types_aiobotocore_quicksight.literals import VisualCustomActionTriggerType

def get_value() -> VisualCustomActionTriggerType:
    return "DATA_POINT_CLICK"
```

```python
# VisualCustomActionTriggerType definition

VisualCustomActionTriggerType = Literal[
    "DATA_POINT_CLICK",
    "DATA_POINT_MENU",
]
```
## WidgetStatusType

```python
# WidgetStatusType usage example

from types_aiobotocore_quicksight.literals import WidgetStatusType

def get_value() -> WidgetStatusType:
    return "DISABLED"
```

```python
# WidgetStatusType definition

WidgetStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## WordCloudCloudLayoutType

```python
# WordCloudCloudLayoutType usage example

from types_aiobotocore_quicksight.literals import WordCloudCloudLayoutType

def get_value() -> WordCloudCloudLayoutType:
    return "FLUID"
```

```python
# WordCloudCloudLayoutType definition

WordCloudCloudLayoutType = Literal[
    "FLUID",
    "NORMAL",
]
```
## WordCloudWordCasingType

```python
# WordCloudWordCasingType usage example

from types_aiobotocore_quicksight.literals import WordCloudWordCasingType

def get_value() -> WordCloudWordCasingType:
    return "EXISTING_CASE"
```

```python
# WordCloudWordCasingType definition

WordCloudWordCasingType = Literal[
    "EXISTING_CASE",
    "LOWER_CASE",
]
```
## WordCloudWordOrientationType

```python
# WordCloudWordOrientationType usage example

from types_aiobotocore_quicksight.literals import WordCloudWordOrientationType

def get_value() -> WordCloudWordOrientationType:
    return "HORIZONTAL"
```

```python
# WordCloudWordOrientationType definition

WordCloudWordOrientationType = Literal[
    "HORIZONTAL",
    "HORIZONTAL_AND_VERTICAL",
]
```
## WordCloudWordPaddingType

```python
# WordCloudWordPaddingType usage example

from types_aiobotocore_quicksight.literals import WordCloudWordPaddingType

def get_value() -> WordCloudWordPaddingType:
    return "LARGE"
```

```python
# WordCloudWordPaddingType definition

WordCloudWordPaddingType = Literal[
    "LARGE",
    "MEDIUM",
    "NONE",
    "SMALL",
]
```
## WordCloudWordScalingType

```python
# WordCloudWordScalingType usage example

from types_aiobotocore_quicksight.literals import WordCloudWordScalingType

def get_value() -> WordCloudWordScalingType:
    return "EMPHASIZE"
```

```python
# WordCloudWordScalingType definition

WordCloudWordScalingType = Literal[
    "EMPHASIZE",
    "NORMAL",
]
```
## QuickSightServiceName

```python
# QuickSightServiceName usage example

from types_aiobotocore_quicksight.literals import QuickSightServiceName

def get_value() -> QuickSightServiceName:
    return "quicksight"
```

```python
# QuickSightServiceName definition

QuickSightServiceName = Literal[
    "quicksight",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_quicksight.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_quicksight.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_quicksight.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_analyses"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_analyses",
    "list_asset_bundle_export_jobs",
    "list_asset_bundle_import_jobs",
    "list_dashboard_versions",
    "list_dashboards",
    "list_data_sets",
    "list_data_sources",
    "list_group_memberships",
    "list_groups",
    "list_iam_policy_assignments",
    "list_iam_policy_assignments_for_user",
    "list_ingestions",
    "list_namespaces",
    "list_template_aliases",
    "list_template_versions",
    "list_templates",
    "list_theme_versions",
    "list_themes",
    "list_user_groups",
    "list_users",
    "search_analyses",
    "search_dashboards",
    "search_data_sets",
    "search_data_sources",
    "search_groups",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_quicksight.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
