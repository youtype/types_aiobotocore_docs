# Type definitions

> [Index](../README.md) > [LookoutMetrics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LookoutMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#lookoutmetrics)
    type annotations stubs module [types-aiobotocore-lookoutmetrics](https://pypi.org/project/types-aiobotocore-lookoutmetrics/).

## CsvFormatDescriptorUnionTypeDef

```python
# CsvFormatDescriptorUnionTypeDef Union usage example

from types_aiobotocore_lookoutmetrics.type_defs import CsvFormatDescriptorUnionTypeDef


def get_value() -> CsvFormatDescriptorUnionTypeDef:
    return ...


# CsvFormatDescriptorUnionTypeDef definition

CsvFormatDescriptorUnionTypeDef = Union[
    CsvFormatDescriptorTypeDef,  # (1)
    CsvFormatDescriptorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CsvFormatDescriptorTypeDef](./type_defs.md#csvformatdescriptortypedef) 
2. See [:material-code-braces: CsvFormatDescriptorOutputTypeDef](./type_defs.md#csvformatdescriptoroutputtypedef) 

## AlertFiltersUnionTypeDef

```python
# AlertFiltersUnionTypeDef Union usage example

from types_aiobotocore_lookoutmetrics.type_defs import AlertFiltersUnionTypeDef


def get_value() -> AlertFiltersUnionTypeDef:
    return ...


# AlertFiltersUnionTypeDef definition

AlertFiltersUnionTypeDef = Union[
    AlertFiltersTypeDef,  # (1)
    AlertFiltersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) 
2. See [:material-code-braces: AlertFiltersOutputTypeDef](./type_defs.md#alertfiltersoutputtypedef) 

## MetricSetDimensionFilterUnionTypeDef

```python
# MetricSetDimensionFilterUnionTypeDef Union usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSetDimensionFilterUnionTypeDef


def get_value() -> MetricSetDimensionFilterUnionTypeDef:
    return ...


# MetricSetDimensionFilterUnionTypeDef definition

MetricSetDimensionFilterUnionTypeDef = Union[
    MetricSetDimensionFilterTypeDef,  # (1)
    MetricSetDimensionFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) 
2. See [:material-code-braces: MetricSetDimensionFilterOutputTypeDef](./type_defs.md#metricsetdimensionfilteroutputtypedef) 

## FileFormatDescriptorUnionTypeDef

```python
# FileFormatDescriptorUnionTypeDef Union usage example

from types_aiobotocore_lookoutmetrics.type_defs import FileFormatDescriptorUnionTypeDef


def get_value() -> FileFormatDescriptorUnionTypeDef:
    return ...


# FileFormatDescriptorUnionTypeDef definition

FileFormatDescriptorUnionTypeDef = Union[
    FileFormatDescriptorTypeDef,  # (1)
    FileFormatDescriptorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FileFormatDescriptorTypeDef](./type_defs.md#fileformatdescriptortypedef) 
2. See [:material-code-braces: FileFormatDescriptorOutputTypeDef](./type_defs.md#fileformatdescriptoroutputtypedef) 

## MetricSourceUnionTypeDef

```python
# MetricSourceUnionTypeDef Union usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSourceUnionTypeDef


def get_value() -> MetricSourceUnionTypeDef:
    return ...


# MetricSourceUnionTypeDef definition

MetricSourceUnionTypeDef = Union[
    MetricSourceTypeDef,  # (1)
    MetricSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) 
2. See [:material-code-braces: MetricSourceOutputTypeDef](./type_defs.md#metricsourceoutputtypedef) 



## LambdaConfigurationTypeDef

```python
# LambdaConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import LambdaConfigurationTypeDef


def get_value() -> LambdaConfigurationTypeDef:
    return {
        "RoleArn": ...,
    }


# LambdaConfigurationTypeDef definition

class LambdaConfigurationTypeDef(TypedDict):
    RoleArn: str,
    LambdaArn: str,
```

## SNSConfigurationTypeDef

```python
# SNSConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import SNSConfigurationTypeDef


def get_value() -> SNSConfigurationTypeDef:
    return {
        "RoleArn": ...,
    }


# SNSConfigurationTypeDef definition

class SNSConfigurationTypeDef(TypedDict):
    RoleArn: str,
    SnsTopicArn: str,
    SnsFormat: NotRequired[SnsFormatType],  # (1)
```

1. See [:material-code-brackets: SnsFormatType](./literals.md#snsformattype) 
## ActivateAnomalyDetectorRequestTypeDef

```python
# ActivateAnomalyDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ActivateAnomalyDetectorRequestTypeDef


def get_value() -> ActivateAnomalyDetectorRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# ActivateAnomalyDetectorRequestTypeDef definition

class ActivateAnomalyDetectorRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DimensionFilterOutputTypeDef

```python
# DimensionFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DimensionFilterOutputTypeDef


def get_value() -> DimensionFilterOutputTypeDef:
    return {
        "DimensionName": ...,
    }


# DimensionFilterOutputTypeDef definition

class DimensionFilterOutputTypeDef(TypedDict):
    DimensionName: NotRequired[str],
    DimensionValueList: NotRequired[List[str]],
```

## DimensionFilterTypeDef

```python
# DimensionFilterTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DimensionFilterTypeDef


def get_value() -> DimensionFilterTypeDef:
    return {
        "DimensionName": ...,
    }


# DimensionFilterTypeDef definition

class DimensionFilterTypeDef(TypedDict):
    DimensionName: NotRequired[str],
    DimensionValueList: NotRequired[Sequence[str]],
```

## AlertSummaryTypeDef

```python
# AlertSummaryTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AlertSummaryTypeDef


def get_value() -> AlertSummaryTypeDef:
    return {
        "AlertArn": ...,
    }


# AlertSummaryTypeDef definition

class AlertSummaryTypeDef(TypedDict):
    AlertArn: NotRequired[str],
    AnomalyDetectorArn: NotRequired[str],
    AlertName: NotRequired[str],
    AlertSensitivityThreshold: NotRequired[int],
    AlertType: NotRequired[AlertTypeType],  # (1)
    AlertStatus: NotRequired[AlertStatusType],  # (2)
    LastModificationTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AlertTypeType](./literals.md#alerttypetype) 
2. See [:material-code-brackets: AlertStatusType](./literals.md#alertstatustype) 
## AnomalyDetectorConfigSummaryTypeDef

```python
# AnomalyDetectorConfigSummaryTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyDetectorConfigSummaryTypeDef


def get_value() -> AnomalyDetectorConfigSummaryTypeDef:
    return {
        "AnomalyDetectorFrequency": ...,
    }


# AnomalyDetectorConfigSummaryTypeDef definition

class AnomalyDetectorConfigSummaryTypeDef(TypedDict):
    AnomalyDetectorFrequency: NotRequired[FrequencyType],  # (1)
```

1. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
## AnomalyDetectorConfigTypeDef

```python
# AnomalyDetectorConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyDetectorConfigTypeDef


def get_value() -> AnomalyDetectorConfigTypeDef:
    return {
        "AnomalyDetectorFrequency": ...,
    }


# AnomalyDetectorConfigTypeDef definition

class AnomalyDetectorConfigTypeDef(TypedDict):
    AnomalyDetectorFrequency: NotRequired[FrequencyType],  # (1)
```

1. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
## AnomalyDetectorSummaryTypeDef

```python
# AnomalyDetectorSummaryTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyDetectorSummaryTypeDef


def get_value() -> AnomalyDetectorSummaryTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# AnomalyDetectorSummaryTypeDef definition

class AnomalyDetectorSummaryTypeDef(TypedDict):
    AnomalyDetectorArn: NotRequired[str],
    AnomalyDetectorName: NotRequired[str],
    AnomalyDetectorDescription: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModificationTime: NotRequired[datetime],
    Status: NotRequired[AnomalyDetectorStatusType],  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AnomalyDetectorStatusType](./literals.md#anomalydetectorstatustype) 
## ItemizedMetricStatsTypeDef

```python
# ItemizedMetricStatsTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ItemizedMetricStatsTypeDef


def get_value() -> ItemizedMetricStatsTypeDef:
    return {
        "MetricName": ...,
    }


# ItemizedMetricStatsTypeDef definition

class ItemizedMetricStatsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    OccurrenceCount: NotRequired[int],
```

## AnomalyGroupSummaryTypeDef

```python
# AnomalyGroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyGroupSummaryTypeDef


def get_value() -> AnomalyGroupSummaryTypeDef:
    return {
        "StartTime": ...,
    }


# AnomalyGroupSummaryTypeDef definition

class AnomalyGroupSummaryTypeDef(TypedDict):
    StartTime: NotRequired[str],
    EndTime: NotRequired[str],
    AnomalyGroupId: NotRequired[str],
    AnomalyGroupScore: NotRequired[float],
    PrimaryMetricName: NotRequired[str],
```

## AnomalyGroupTimeSeriesFeedbackTypeDef

```python
# AnomalyGroupTimeSeriesFeedbackTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyGroupTimeSeriesFeedbackTypeDef


def get_value() -> AnomalyGroupTimeSeriesFeedbackTypeDef:
    return {
        "AnomalyGroupId": ...,
    }


# AnomalyGroupTimeSeriesFeedbackTypeDef definition

class AnomalyGroupTimeSeriesFeedbackTypeDef(TypedDict):
    AnomalyGroupId: str,
    TimeSeriesId: str,
    IsAnomaly: bool,
```

## AnomalyGroupTimeSeriesTypeDef

```python
# AnomalyGroupTimeSeriesTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyGroupTimeSeriesTypeDef


def get_value() -> AnomalyGroupTimeSeriesTypeDef:
    return {
        "AnomalyGroupId": ...,
    }


# AnomalyGroupTimeSeriesTypeDef definition

class AnomalyGroupTimeSeriesTypeDef(TypedDict):
    AnomalyGroupId: str,
    TimeSeriesId: NotRequired[str],
```

## AppFlowConfigTypeDef

```python
# AppFlowConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AppFlowConfigTypeDef


def get_value() -> AppFlowConfigTypeDef:
    return {
        "RoleArn": ...,
    }


# AppFlowConfigTypeDef definition

class AppFlowConfigTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    FlowName: NotRequired[str],
```

## BackTestConfigurationTypeDef

```python
# BackTestConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import BackTestConfigurationTypeDef


def get_value() -> BackTestConfigurationTypeDef:
    return {
        "RunBackTestMode": ...,
    }


# BackTestConfigurationTypeDef definition

class BackTestConfigurationTypeDef(TypedDict):
    RunBackTestMode: bool,
```

## AttributeValueTypeDef

```python
# AttributeValueTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AttributeValueTypeDef


def get_value() -> AttributeValueTypeDef:
    return {
        "S": ...,
    }


# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    S: NotRequired[str],
    N: NotRequired[str],
    B: NotRequired[str],
    SS: NotRequired[List[str]],
    NS: NotRequired[List[str]],
    BS: NotRequired[List[str]],
```

## AutoDetectionS3SourceConfigTypeDef

```python
# AutoDetectionS3SourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AutoDetectionS3SourceConfigTypeDef


def get_value() -> AutoDetectionS3SourceConfigTypeDef:
    return {
        "TemplatedPathList": ...,
    }


# AutoDetectionS3SourceConfigTypeDef definition

class AutoDetectionS3SourceConfigTypeDef(TypedDict):
    TemplatedPathList: NotRequired[Sequence[str]],
    HistoricalDataPathList: NotRequired[Sequence[str]],
```

## BackTestAnomalyDetectorRequestTypeDef

```python
# BackTestAnomalyDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import BackTestAnomalyDetectorRequestTypeDef


def get_value() -> BackTestAnomalyDetectorRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# BackTestAnomalyDetectorRequestTypeDef definition

class BackTestAnomalyDetectorRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## MetricTypeDef

```python
# MetricTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricTypeDef


def get_value() -> MetricTypeDef:
    return {
        "MetricName": ...,
    }


# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    MetricName: str,
    AggregationFunction: AggregationFunctionType,  # (1)
    Namespace: NotRequired[str],
```

1. See [:material-code-brackets: AggregationFunctionType](./literals.md#aggregationfunctiontype) 
## TimestampColumnTypeDef

```python
# TimestampColumnTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import TimestampColumnTypeDef


def get_value() -> TimestampColumnTypeDef:
    return {
        "ColumnName": ...,
    }


# TimestampColumnTypeDef definition

class TimestampColumnTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    ColumnFormat: NotRequired[str],
```

## CsvFormatDescriptorOutputTypeDef

```python
# CsvFormatDescriptorOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CsvFormatDescriptorOutputTypeDef


def get_value() -> CsvFormatDescriptorOutputTypeDef:
    return {
        "FileCompression": ...,
    }


# CsvFormatDescriptorOutputTypeDef definition

class CsvFormatDescriptorOutputTypeDef(TypedDict):
    FileCompression: NotRequired[CSVFileCompressionType],  # (1)
    Charset: NotRequired[str],
    ContainsHeader: NotRequired[bool],
    Delimiter: NotRequired[str],
    HeaderList: NotRequired[List[str]],
    QuoteSymbol: NotRequired[str],
```

1. See [:material-code-brackets: CSVFileCompressionType](./literals.md#csvfilecompressiontype) 
## CsvFormatDescriptorTypeDef

```python
# CsvFormatDescriptorTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CsvFormatDescriptorTypeDef


def get_value() -> CsvFormatDescriptorTypeDef:
    return {
        "FileCompression": ...,
    }


# CsvFormatDescriptorTypeDef definition

class CsvFormatDescriptorTypeDef(TypedDict):
    FileCompression: NotRequired[CSVFileCompressionType],  # (1)
    Charset: NotRequired[str],
    ContainsHeader: NotRequired[bool],
    Delimiter: NotRequired[str],
    HeaderList: NotRequired[Sequence[str]],
    QuoteSymbol: NotRequired[str],
```

1. See [:material-code-brackets: CSVFileCompressionType](./literals.md#csvfilecompressiontype) 
## DataQualityMetricTypeDef

```python
# DataQualityMetricTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DataQualityMetricTypeDef


def get_value() -> DataQualityMetricTypeDef:
    return {
        "MetricType": ...,
    }


# DataQualityMetricTypeDef definition

class DataQualityMetricTypeDef(TypedDict):
    MetricType: NotRequired[DataQualityMetricTypeType],  # (1)
    MetricDescription: NotRequired[str],
    RelatedColumnName: NotRequired[str],
    MetricValue: NotRequired[float],
```

1. See [:material-code-brackets: DataQualityMetricTypeType](./literals.md#dataqualitymetrictypetype) 
## DeactivateAnomalyDetectorRequestTypeDef

```python
# DeactivateAnomalyDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DeactivateAnomalyDetectorRequestTypeDef


def get_value() -> DeactivateAnomalyDetectorRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# DeactivateAnomalyDetectorRequestTypeDef definition

class DeactivateAnomalyDetectorRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DeleteAlertRequestTypeDef

```python
# DeleteAlertRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DeleteAlertRequestTypeDef


def get_value() -> DeleteAlertRequestTypeDef:
    return {
        "AlertArn": ...,
    }


# DeleteAlertRequestTypeDef definition

class DeleteAlertRequestTypeDef(TypedDict):
    AlertArn: str,
```

## DeleteAnomalyDetectorRequestTypeDef

```python
# DeleteAnomalyDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DeleteAnomalyDetectorRequestTypeDef


def get_value() -> DeleteAnomalyDetectorRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# DeleteAnomalyDetectorRequestTypeDef definition

class DeleteAnomalyDetectorRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DescribeAlertRequestTypeDef

```python
# DescribeAlertRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeAlertRequestTypeDef


def get_value() -> DescribeAlertRequestTypeDef:
    return {
        "AlertArn": ...,
    }


# DescribeAlertRequestTypeDef definition

class DescribeAlertRequestTypeDef(TypedDict):
    AlertArn: str,
```

## DescribeAnomalyDetectionExecutionsRequestTypeDef

```python
# DescribeAnomalyDetectionExecutionsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeAnomalyDetectionExecutionsRequestTypeDef


def get_value() -> DescribeAnomalyDetectionExecutionsRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# DescribeAnomalyDetectionExecutionsRequestTypeDef definition

class DescribeAnomalyDetectionExecutionsRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    Timestamp: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ExecutionStatusTypeDef

```python
# ExecutionStatusTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ExecutionStatusTypeDef


def get_value() -> ExecutionStatusTypeDef:
    return {
        "Timestamp": ...,
    }


# ExecutionStatusTypeDef definition

class ExecutionStatusTypeDef(TypedDict):
    Timestamp: NotRequired[str],
    Status: NotRequired[AnomalyDetectionTaskStatusType],  # (1)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: AnomalyDetectionTaskStatusType](./literals.md#anomalydetectiontaskstatustype) 
## DescribeAnomalyDetectorRequestTypeDef

```python
# DescribeAnomalyDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeAnomalyDetectorRequestTypeDef


def get_value() -> DescribeAnomalyDetectorRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# DescribeAnomalyDetectorRequestTypeDef definition

class DescribeAnomalyDetectorRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DescribeMetricSetRequestTypeDef

```python
# DescribeMetricSetRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeMetricSetRequestTypeDef


def get_value() -> DescribeMetricSetRequestTypeDef:
    return {
        "MetricSetArn": ...,
    }


# DescribeMetricSetRequestTypeDef definition

class DescribeMetricSetRequestTypeDef(TypedDict):
    MetricSetArn: str,
```

## DimensionValueContributionTypeDef

```python
# DimensionValueContributionTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DimensionValueContributionTypeDef


def get_value() -> DimensionValueContributionTypeDef:
    return {
        "DimensionValue": ...,
    }


# DimensionValueContributionTypeDef definition

class DimensionValueContributionTypeDef(TypedDict):
    DimensionValue: NotRequired[str],
    ContributionScore: NotRequired[float],
```

## DimensionNameValueTypeDef

```python
# DimensionNameValueTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DimensionNameValueTypeDef


def get_value() -> DimensionNameValueTypeDef:
    return {
        "DimensionName": ...,
    }


# DimensionNameValueTypeDef definition

class DimensionNameValueTypeDef(TypedDict):
    DimensionName: str,
    DimensionValue: str,
```

## JsonFormatDescriptorTypeDef

```python
# JsonFormatDescriptorTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import JsonFormatDescriptorTypeDef


def get_value() -> JsonFormatDescriptorTypeDef:
    return {
        "FileCompression": ...,
    }


# JsonFormatDescriptorTypeDef definition

class JsonFormatDescriptorTypeDef(TypedDict):
    FileCompression: NotRequired[JsonFileCompressionType],  # (1)
    Charset: NotRequired[str],
```

1. See [:material-code-brackets: JsonFileCompressionType](./literals.md#jsonfilecompressiontype) 
## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "DimensionValue": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    DimensionValue: NotRequired[str],
    FilterOperation: NotRequired[FilterOperationType],  # (1)
```

1. See [:material-code-brackets: FilterOperationType](./literals.md#filteroperationtype) 
## GetAnomalyGroupRequestTypeDef

```python
# GetAnomalyGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetAnomalyGroupRequestTypeDef


def get_value() -> GetAnomalyGroupRequestTypeDef:
    return {
        "AnomalyGroupId": ...,
    }


# GetAnomalyGroupRequestTypeDef definition

class GetAnomalyGroupRequestTypeDef(TypedDict):
    AnomalyGroupId: str,
    AnomalyDetectorArn: str,
```

## GetDataQualityMetricsRequestTypeDef

```python
# GetDataQualityMetricsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetDataQualityMetricsRequestTypeDef


def get_value() -> GetDataQualityMetricsRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# GetDataQualityMetricsRequestTypeDef definition

class GetDataQualityMetricsRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    MetricSetArn: NotRequired[str],
```

## TimeSeriesFeedbackTypeDef

```python
# TimeSeriesFeedbackTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import TimeSeriesFeedbackTypeDef


def get_value() -> TimeSeriesFeedbackTypeDef:
    return {
        "TimeSeriesId": ...,
    }


# TimeSeriesFeedbackTypeDef definition

class TimeSeriesFeedbackTypeDef(TypedDict):
    TimeSeriesId: NotRequired[str],
    IsAnomaly: NotRequired[bool],
```

## InterMetricImpactDetailsTypeDef

```python
# InterMetricImpactDetailsTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import InterMetricImpactDetailsTypeDef


def get_value() -> InterMetricImpactDetailsTypeDef:
    return {
        "MetricName": ...,
    }


# InterMetricImpactDetailsTypeDef definition

class InterMetricImpactDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    AnomalyGroupId: NotRequired[str],
    RelationshipType: NotRequired[RelationshipTypeType],  # (1)
    ContributionPercentage: NotRequired[float],
```

1. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
## ListAlertsRequestTypeDef

```python
# ListAlertsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAlertsRequestTypeDef


def get_value() -> ListAlertsRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# ListAlertsRequestTypeDef definition

class ListAlertsRequestTypeDef(TypedDict):
    AnomalyDetectorArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAnomalyDetectorsRequestTypeDef

```python
# ListAnomalyDetectorsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyDetectorsRequestTypeDef


def get_value() -> ListAnomalyDetectorsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListAnomalyDetectorsRequestTypeDef definition

class ListAnomalyDetectorsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAnomalyGroupRelatedMetricsRequestTypeDef

```python
# ListAnomalyGroupRelatedMetricsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyGroupRelatedMetricsRequestTypeDef


def get_value() -> ListAnomalyGroupRelatedMetricsRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# ListAnomalyGroupRelatedMetricsRequestTypeDef definition

class ListAnomalyGroupRelatedMetricsRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupId: str,
    RelationshipTypeFilter: NotRequired[RelationshipTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
## ListAnomalyGroupSummariesRequestTypeDef

```python
# ListAnomalyGroupSummariesRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyGroupSummariesRequestTypeDef


def get_value() -> ListAnomalyGroupSummariesRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# ListAnomalyGroupSummariesRequestTypeDef definition

class ListAnomalyGroupSummariesRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    SensitivityThreshold: int,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAnomalyGroupTimeSeriesRequestTypeDef

```python
# ListAnomalyGroupTimeSeriesRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyGroupTimeSeriesRequestTypeDef


def get_value() -> ListAnomalyGroupTimeSeriesRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# ListAnomalyGroupTimeSeriesRequestTypeDef definition

class ListAnomalyGroupTimeSeriesRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupId: str,
    MetricName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMetricSetsRequestTypeDef

```python
# ListMetricSetsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListMetricSetsRequestTypeDef


def get_value() -> ListMetricSetsRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# ListMetricSetsRequestTypeDef definition

class ListMetricSetsRequestTypeDef(TypedDict):
    AnomalyDetectorArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MetricSetSummaryTypeDef

```python
# MetricSetSummaryTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSetSummaryTypeDef


def get_value() -> MetricSetSummaryTypeDef:
    return {
        "MetricSetArn": ...,
    }


# MetricSetSummaryTypeDef definition

class MetricSetSummaryTypeDef(TypedDict):
    MetricSetArn: NotRequired[str],
    AnomalyDetectorArn: NotRequired[str],
    MetricSetDescription: NotRequired[str],
    MetricSetName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModificationTime: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## VpcConfigurationOutputTypeDef

```python
# VpcConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import VpcConfigurationOutputTypeDef


def get_value() -> VpcConfigurationOutputTypeDef:
    return {
        "SubnetIdList": ...,
    }


# VpcConfigurationOutputTypeDef definition

class VpcConfigurationOutputTypeDef(TypedDict):
    SubnetIdList: List[str],
    SecurityGroupIdList: List[str],
```

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import VpcConfigurationTypeDef


def get_value() -> VpcConfigurationTypeDef:
    return {
        "SubnetIdList": ...,
    }


# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    SubnetIdList: Sequence[str],
    SecurityGroupIdList: Sequence[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ActionTypeDef

```python
# ActionTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ActionTypeDef


def get_value() -> ActionTypeDef:
    return {
        "SNSConfiguration": ...,
    }


# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    SNSConfiguration: NotRequired[SNSConfigurationTypeDef],  # (1)
    LambdaConfiguration: NotRequired[LambdaConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: SNSConfigurationTypeDef](./type_defs.md#snsconfigurationtypedef) 
2. See [:material-code-braces: LambdaConfigurationTypeDef](./type_defs.md#lambdaconfigurationtypedef) 
## AlertFiltersOutputTypeDef

```python
# AlertFiltersOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AlertFiltersOutputTypeDef


def get_value() -> AlertFiltersOutputTypeDef:
    return {
        "MetricList": ...,
    }


# AlertFiltersOutputTypeDef definition

class AlertFiltersOutputTypeDef(TypedDict):
    MetricList: NotRequired[List[str]],
    DimensionFilterList: NotRequired[List[DimensionFilterOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFilterOutputTypeDef](./type_defs.md#dimensionfilteroutputtypedef) 
## AlertFiltersTypeDef

```python
# AlertFiltersTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AlertFiltersTypeDef


def get_value() -> AlertFiltersTypeDef:
    return {
        "MetricList": ...,
    }


# AlertFiltersTypeDef definition

class AlertFiltersTypeDef(TypedDict):
    MetricList: NotRequired[Sequence[str]],
    DimensionFilterList: NotRequired[Sequence[DimensionFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef) 
## CreateAnomalyDetectorRequestTypeDef

```python
# CreateAnomalyDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CreateAnomalyDetectorRequestTypeDef


def get_value() -> CreateAnomalyDetectorRequestTypeDef:
    return {
        "AnomalyDetectorName": ...,
    }


# CreateAnomalyDetectorRequestTypeDef definition

class CreateAnomalyDetectorRequestTypeDef(TypedDict):
    AnomalyDetectorName: str,
    AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef,  # (1)
    AnomalyDetectorDescription: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AnomalyDetectorConfigTypeDef](./type_defs.md#anomalydetectorconfigtypedef) 
## UpdateAnomalyDetectorRequestTypeDef

```python
# UpdateAnomalyDetectorRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import UpdateAnomalyDetectorRequestTypeDef


def get_value() -> UpdateAnomalyDetectorRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# UpdateAnomalyDetectorRequestTypeDef definition

class UpdateAnomalyDetectorRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    KmsKeyArn: NotRequired[str],
    AnomalyDetectorDescription: NotRequired[str],
    AnomalyDetectorConfig: NotRequired[AnomalyDetectorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AnomalyDetectorConfigTypeDef](./type_defs.md#anomalydetectorconfigtypedef) 
## AnomalyGroupStatisticsTypeDef

```python
# AnomalyGroupStatisticsTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyGroupStatisticsTypeDef


def get_value() -> AnomalyGroupStatisticsTypeDef:
    return {
        "EvaluationStartDate": ...,
    }


# AnomalyGroupStatisticsTypeDef definition

class AnomalyGroupStatisticsTypeDef(TypedDict):
    EvaluationStartDate: NotRequired[str],
    TotalCount: NotRequired[int],
    ItemizedMetricStatsList: NotRequired[List[ItemizedMetricStatsTypeDef]],  # (1)
```

1. See [:material-code-braces: ItemizedMetricStatsTypeDef](./type_defs.md#itemizedmetricstatstypedef) 
## PutFeedbackRequestTypeDef

```python
# PutFeedbackRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import PutFeedbackRequestTypeDef


def get_value() -> PutFeedbackRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# PutFeedbackRequestTypeDef definition

class PutFeedbackRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesFeedbackTypeDef,  # (1)
```

1. See [:material-code-braces: AnomalyGroupTimeSeriesFeedbackTypeDef](./type_defs.md#anomalygrouptimeseriesfeedbacktypedef) 
## GetFeedbackRequestTypeDef

```python
# GetFeedbackRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetFeedbackRequestTypeDef


def get_value() -> GetFeedbackRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# GetFeedbackRequestTypeDef definition

class GetFeedbackRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnomalyGroupTimeSeriesTypeDef](./type_defs.md#anomalygrouptimeseriestypedef) 
## AthenaSourceConfigTypeDef

```python
# AthenaSourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AthenaSourceConfigTypeDef


def get_value() -> AthenaSourceConfigTypeDef:
    return {
        "RoleArn": ...,
    }


# AthenaSourceConfigTypeDef definition

class AthenaSourceConfigTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    DatabaseName: NotRequired[str],
    DataCatalog: NotRequired[str],
    TableName: NotRequired[str],
    WorkGroupName: NotRequired[str],
    S3ResultsPath: NotRequired[str],
    BackTestConfiguration: NotRequired[BackTestConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: BackTestConfigurationTypeDef](./type_defs.md#backtestconfigurationtypedef) 
## CloudWatchConfigTypeDef

```python
# CloudWatchConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CloudWatchConfigTypeDef


def get_value() -> CloudWatchConfigTypeDef:
    return {
        "RoleArn": ...,
    }


# CloudWatchConfigTypeDef definition

class CloudWatchConfigTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    BackTestConfiguration: NotRequired[BackTestConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: BackTestConfigurationTypeDef](./type_defs.md#backtestconfigurationtypedef) 
## DetectedFieldTypeDef

```python
# DetectedFieldTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectedFieldTypeDef


def get_value() -> DetectedFieldTypeDef:
    return {
        "Value": ...,
    }


# DetectedFieldTypeDef definition

class DetectedFieldTypeDef(TypedDict):
    Value: NotRequired[AttributeValueTypeDef],  # (1)
    Confidence: NotRequired[ConfidenceType],  # (2)
    Message: NotRequired[str],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ConfidenceType](./literals.md#confidencetype) 
## AutoDetectionMetricSourceTypeDef

```python
# AutoDetectionMetricSourceTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AutoDetectionMetricSourceTypeDef


def get_value() -> AutoDetectionMetricSourceTypeDef:
    return {
        "S3SourceConfig": ...,
    }


# AutoDetectionMetricSourceTypeDef definition

class AutoDetectionMetricSourceTypeDef(TypedDict):
    S3SourceConfig: NotRequired[AutoDetectionS3SourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AutoDetectionS3SourceConfigTypeDef](./type_defs.md#autodetections3sourceconfigtypedef) 
## CreateAlertResponseTypeDef

```python
# CreateAlertResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CreateAlertResponseTypeDef


def get_value() -> CreateAlertResponseTypeDef:
    return {
        "AlertArn": ...,
    }


# CreateAlertResponseTypeDef definition

class CreateAlertResponseTypeDef(TypedDict):
    AlertArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAnomalyDetectorResponseTypeDef

```python
# CreateAnomalyDetectorResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CreateAnomalyDetectorResponseTypeDef


def get_value() -> CreateAnomalyDetectorResponseTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# CreateAnomalyDetectorResponseTypeDef definition

class CreateAnomalyDetectorResponseTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMetricSetResponseTypeDef

```python
# CreateMetricSetResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CreateMetricSetResponseTypeDef


def get_value() -> CreateMetricSetResponseTypeDef:
    return {
        "MetricSetArn": ...,
    }


# CreateMetricSetResponseTypeDef definition

class CreateMetricSetResponseTypeDef(TypedDict):
    MetricSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAnomalyDetectorResponseTypeDef

```python
# DescribeAnomalyDetectorResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeAnomalyDetectorResponseTypeDef


def get_value() -> DescribeAnomalyDetectorResponseTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# DescribeAnomalyDetectorResponseTypeDef definition

class DescribeAnomalyDetectorResponseTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyDetectorName: str,
    AnomalyDetectorDescription: str,
    AnomalyDetectorConfig: AnomalyDetectorConfigSummaryTypeDef,  # (1)
    CreationTime: datetime,
    LastModificationTime: datetime,
    Status: AnomalyDetectorStatusType,  # (2)
    FailureReason: str,
    KmsKeyArn: str,
    FailureType: AnomalyDetectorFailureTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AnomalyDetectorConfigSummaryTypeDef](./type_defs.md#anomalydetectorconfigsummarytypedef) 
2. See [:material-code-brackets: AnomalyDetectorStatusType](./literals.md#anomalydetectorstatustype) 
3. See [:material-code-brackets: AnomalyDetectorFailureTypeType](./literals.md#anomalydetectorfailuretypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSampleDataResponseTypeDef

```python
# GetSampleDataResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetSampleDataResponseTypeDef


def get_value() -> GetSampleDataResponseTypeDef:
    return {
        "HeaderValues": ...,
    }


# GetSampleDataResponseTypeDef definition

class GetSampleDataResponseTypeDef(TypedDict):
    HeaderValues: List[str],
    SampleRows: List[List[str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlertsResponseTypeDef

```python
# ListAlertsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAlertsResponseTypeDef


def get_value() -> ListAlertsResponseTypeDef:
    return {
        "AlertSummaryList": ...,
    }


# ListAlertsResponseTypeDef definition

class ListAlertsResponseTypeDef(TypedDict):
    AlertSummaryList: List[AlertSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AlertSummaryTypeDef](./type_defs.md#alertsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnomalyDetectorsResponseTypeDef

```python
# ListAnomalyDetectorsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyDetectorsResponseTypeDef


def get_value() -> ListAnomalyDetectorsResponseTypeDef:
    return {
        "AnomalyDetectorSummaryList": ...,
    }


# ListAnomalyDetectorsResponseTypeDef definition

class ListAnomalyDetectorsResponseTypeDef(TypedDict):
    AnomalyDetectorSummaryList: List[AnomalyDetectorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnomalyDetectorSummaryTypeDef](./type_defs.md#anomalydetectorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAlertResponseTypeDef

```python
# UpdateAlertResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import UpdateAlertResponseTypeDef


def get_value() -> UpdateAlertResponseTypeDef:
    return {
        "AlertArn": ...,
    }


# UpdateAlertResponseTypeDef definition

class UpdateAlertResponseTypeDef(TypedDict):
    AlertArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnomalyDetectorResponseTypeDef

```python
# UpdateAnomalyDetectorResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import UpdateAnomalyDetectorResponseTypeDef


def get_value() -> UpdateAnomalyDetectorResponseTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# UpdateAnomalyDetectorResponseTypeDef definition

class UpdateAnomalyDetectorResponseTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMetricSetResponseTypeDef

```python
# UpdateMetricSetResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import UpdateMetricSetResponseTypeDef


def get_value() -> UpdateMetricSetResponseTypeDef:
    return {
        "MetricSetArn": ...,
    }


# UpdateMetricSetResponseTypeDef definition

class UpdateMetricSetResponseTypeDef(TypedDict):
    MetricSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricSetDataQualityMetricTypeDef

```python
# MetricSetDataQualityMetricTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSetDataQualityMetricTypeDef


def get_value() -> MetricSetDataQualityMetricTypeDef:
    return {
        "MetricSetArn": ...,
    }


# MetricSetDataQualityMetricTypeDef definition

class MetricSetDataQualityMetricTypeDef(TypedDict):
    MetricSetArn: NotRequired[str],
    DataQualityMetricList: NotRequired[List[DataQualityMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: DataQualityMetricTypeDef](./type_defs.md#dataqualitymetrictypedef) 
## DescribeAnomalyDetectionExecutionsResponseTypeDef

```python
# DescribeAnomalyDetectionExecutionsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeAnomalyDetectionExecutionsResponseTypeDef


def get_value() -> DescribeAnomalyDetectionExecutionsResponseTypeDef:
    return {
        "ExecutionList": ...,
    }


# DescribeAnomalyDetectionExecutionsResponseTypeDef definition

class DescribeAnomalyDetectionExecutionsResponseTypeDef(TypedDict):
    ExecutionList: List[ExecutionStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExecutionStatusTypeDef](./type_defs.md#executionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DimensionContributionTypeDef

```python
# DimensionContributionTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DimensionContributionTypeDef


def get_value() -> DimensionContributionTypeDef:
    return {
        "DimensionName": ...,
    }


# DimensionContributionTypeDef definition

class DimensionContributionTypeDef(TypedDict):
    DimensionName: NotRequired[str],
    DimensionValueContributionList: NotRequired[List[DimensionValueContributionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionValueContributionTypeDef](./type_defs.md#dimensionvaluecontributiontypedef) 
## TimeSeriesTypeDef

```python
# TimeSeriesTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import TimeSeriesTypeDef


def get_value() -> TimeSeriesTypeDef:
    return {
        "TimeSeriesId": ...,
    }


# TimeSeriesTypeDef definition

class TimeSeriesTypeDef(TypedDict):
    TimeSeriesId: str,
    DimensionList: List[DimensionNameValueTypeDef],  # (1)
    MetricValueList: List[float],
```

1. See [:material-code-braces: DimensionNameValueTypeDef](./type_defs.md#dimensionnamevaluetypedef) 
## FileFormatDescriptorOutputTypeDef

```python
# FileFormatDescriptorOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import FileFormatDescriptorOutputTypeDef


def get_value() -> FileFormatDescriptorOutputTypeDef:
    return {
        "CsvFormatDescriptor": ...,
    }


# FileFormatDescriptorOutputTypeDef definition

class FileFormatDescriptorOutputTypeDef(TypedDict):
    CsvFormatDescriptor: NotRequired[CsvFormatDescriptorOutputTypeDef],  # (1)
    JsonFormatDescriptor: NotRequired[JsonFormatDescriptorTypeDef],  # (2)
```

1. See [:material-code-braces: CsvFormatDescriptorOutputTypeDef](./type_defs.md#csvformatdescriptoroutputtypedef) 
2. See [:material-code-braces: JsonFormatDescriptorTypeDef](./type_defs.md#jsonformatdescriptortypedef) 
## MetricSetDimensionFilterOutputTypeDef

```python
# MetricSetDimensionFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSetDimensionFilterOutputTypeDef


def get_value() -> MetricSetDimensionFilterOutputTypeDef:
    return {
        "Name": ...,
    }


# MetricSetDimensionFilterOutputTypeDef definition

class MetricSetDimensionFilterOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    FilterList: NotRequired[List[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## MetricSetDimensionFilterTypeDef

```python
# MetricSetDimensionFilterTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSetDimensionFilterTypeDef


def get_value() -> MetricSetDimensionFilterTypeDef:
    return {
        "Name": ...,
    }


# MetricSetDimensionFilterTypeDef definition

class MetricSetDimensionFilterTypeDef(TypedDict):
    Name: NotRequired[str],
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetFeedbackResponseTypeDef

```python
# GetFeedbackResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetFeedbackResponseTypeDef


def get_value() -> GetFeedbackResponseTypeDef:
    return {
        "AnomalyGroupTimeSeriesFeedback": ...,
    }


# GetFeedbackResponseTypeDef definition

class GetFeedbackResponseTypeDef(TypedDict):
    AnomalyGroupTimeSeriesFeedback: List[TimeSeriesFeedbackTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeSeriesFeedbackTypeDef](./type_defs.md#timeseriesfeedbacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnomalyGroupRelatedMetricsResponseTypeDef

```python
# ListAnomalyGroupRelatedMetricsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyGroupRelatedMetricsResponseTypeDef


def get_value() -> ListAnomalyGroupRelatedMetricsResponseTypeDef:
    return {
        "InterMetricImpactList": ...,
    }


# ListAnomalyGroupRelatedMetricsResponseTypeDef definition

class ListAnomalyGroupRelatedMetricsResponseTypeDef(TypedDict):
    InterMetricImpactList: List[InterMetricImpactDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InterMetricImpactDetailsTypeDef](./type_defs.md#intermetricimpactdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMetricSetsResponseTypeDef

```python
# ListMetricSetsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListMetricSetsResponseTypeDef


def get_value() -> ListMetricSetsResponseTypeDef:
    return {
        "MetricSetSummaryList": ...,
    }


# ListMetricSetsResponseTypeDef definition

class ListMetricSetsResponseTypeDef(TypedDict):
    MetricSetSummaryList: List[MetricSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MetricSetSummaryTypeDef](./type_defs.md#metricsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RDSSourceConfigOutputTypeDef

```python
# RDSSourceConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import RDSSourceConfigOutputTypeDef


def get_value() -> RDSSourceConfigOutputTypeDef:
    return {
        "DBInstanceIdentifier": ...,
    }


# RDSSourceConfigOutputTypeDef definition

class RDSSourceConfigOutputTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DatabaseHost: NotRequired[str],
    DatabasePort: NotRequired[int],
    SecretManagerArn: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    RoleArn: NotRequired[str],
    VpcConfiguration: NotRequired[VpcConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
## RedshiftSourceConfigOutputTypeDef

```python
# RedshiftSourceConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import RedshiftSourceConfigOutputTypeDef


def get_value() -> RedshiftSourceConfigOutputTypeDef:
    return {
        "ClusterIdentifier": ...,
    }


# RedshiftSourceConfigOutputTypeDef definition

class RedshiftSourceConfigOutputTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    DatabaseHost: NotRequired[str],
    DatabasePort: NotRequired[int],
    SecretManagerArn: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    RoleArn: NotRequired[str],
    VpcConfiguration: NotRequired[VpcConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
## RDSSourceConfigTypeDef

```python
# RDSSourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import RDSSourceConfigTypeDef


def get_value() -> RDSSourceConfigTypeDef:
    return {
        "DBInstanceIdentifier": ...,
    }


# RDSSourceConfigTypeDef definition

class RDSSourceConfigTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DatabaseHost: NotRequired[str],
    DatabasePort: NotRequired[int],
    SecretManagerArn: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    RoleArn: NotRequired[str],
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
## RedshiftSourceConfigTypeDef

```python
# RedshiftSourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import RedshiftSourceConfigTypeDef


def get_value() -> RedshiftSourceConfigTypeDef:
    return {
        "ClusterIdentifier": ...,
    }


# RedshiftSourceConfigTypeDef definition

class RedshiftSourceConfigTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    DatabaseHost: NotRequired[str],
    DatabasePort: NotRequired[int],
    SecretManagerArn: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    RoleArn: NotRequired[str],
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
## AlertTypeDef

```python
# AlertTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AlertTypeDef


def get_value() -> AlertTypeDef:
    return {
        "Action": ...,
    }


# AlertTypeDef definition

class AlertTypeDef(TypedDict):
    Action: NotRequired[ActionTypeDef],  # (1)
    AlertDescription: NotRequired[str],
    AlertArn: NotRequired[str],
    AnomalyDetectorArn: NotRequired[str],
    AlertName: NotRequired[str],
    AlertSensitivityThreshold: NotRequired[int],
    AlertType: NotRequired[AlertTypeType],  # (2)
    AlertStatus: NotRequired[AlertStatusType],  # (3)
    LastModificationTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    AlertFilters: NotRequired[AlertFiltersOutputTypeDef],  # (4)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-brackets: AlertTypeType](./literals.md#alerttypetype) 
3. See [:material-code-brackets: AlertStatusType](./literals.md#alertstatustype) 
4. See [:material-code-braces: AlertFiltersOutputTypeDef](./type_defs.md#alertfiltersoutputtypedef) 
## ListAnomalyGroupSummariesResponseTypeDef

```python
# ListAnomalyGroupSummariesResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyGroupSummariesResponseTypeDef


def get_value() -> ListAnomalyGroupSummariesResponseTypeDef:
    return {
        "AnomalyGroupSummaryList": ...,
    }


# ListAnomalyGroupSummariesResponseTypeDef definition

class ListAnomalyGroupSummariesResponseTypeDef(TypedDict):
    AnomalyGroupSummaryList: List[AnomalyGroupSummaryTypeDef],  # (1)
    AnomalyGroupStatistics: AnomalyGroupStatisticsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnomalyGroupSummaryTypeDef](./type_defs.md#anomalygroupsummarytypedef) 
2. See [:material-code-braces: AnomalyGroupStatisticsTypeDef](./type_defs.md#anomalygroupstatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectedCsvFormatDescriptorTypeDef

```python
# DetectedCsvFormatDescriptorTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectedCsvFormatDescriptorTypeDef


def get_value() -> DetectedCsvFormatDescriptorTypeDef:
    return {
        "FileCompression": ...,
    }


# DetectedCsvFormatDescriptorTypeDef definition

class DetectedCsvFormatDescriptorTypeDef(TypedDict):
    FileCompression: NotRequired[DetectedFieldTypeDef],  # (1)
    Charset: NotRequired[DetectedFieldTypeDef],  # (1)
    ContainsHeader: NotRequired[DetectedFieldTypeDef],  # (1)
    Delimiter: NotRequired[DetectedFieldTypeDef],  # (1)
    HeaderList: NotRequired[DetectedFieldTypeDef],  # (1)
    QuoteSymbol: NotRequired[DetectedFieldTypeDef],  # (1)
```

1. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
2. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
3. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
4. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
5. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
6. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
## DetectedJsonFormatDescriptorTypeDef

```python
# DetectedJsonFormatDescriptorTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectedJsonFormatDescriptorTypeDef


def get_value() -> DetectedJsonFormatDescriptorTypeDef:
    return {
        "FileCompression": ...,
    }


# DetectedJsonFormatDescriptorTypeDef definition

class DetectedJsonFormatDescriptorTypeDef(TypedDict):
    FileCompression: NotRequired[DetectedFieldTypeDef],  # (1)
    Charset: NotRequired[DetectedFieldTypeDef],  # (1)
```

1. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
2. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
## DetectMetricSetConfigRequestTypeDef

```python
# DetectMetricSetConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectMetricSetConfigRequestTypeDef


def get_value() -> DetectMetricSetConfigRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# DetectMetricSetConfigRequestTypeDef definition

class DetectMetricSetConfigRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AutoDetectionMetricSource: AutoDetectionMetricSourceTypeDef,  # (1)
```

1. See [:material-code-braces: AutoDetectionMetricSourceTypeDef](./type_defs.md#autodetectionmetricsourcetypedef) 
## FileFormatDescriptorTypeDef

```python
# FileFormatDescriptorTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import FileFormatDescriptorTypeDef


def get_value() -> FileFormatDescriptorTypeDef:
    return {
        "CsvFormatDescriptor": ...,
    }


# FileFormatDescriptorTypeDef definition

class FileFormatDescriptorTypeDef(TypedDict):
    CsvFormatDescriptor: NotRequired[CsvFormatDescriptorUnionTypeDef],  # (1)
    JsonFormatDescriptor: NotRequired[JsonFormatDescriptorTypeDef],  # (2)
```

1. See [:material-code-braces: CsvFormatDescriptorTypeDef](./type_defs.md#csvformatdescriptortypedef) [:material-code-braces: CsvFormatDescriptorOutputTypeDef](./type_defs.md#csvformatdescriptoroutputtypedef) 
2. See [:material-code-braces: JsonFormatDescriptorTypeDef](./type_defs.md#jsonformatdescriptortypedef) 
## AnomalyDetectorDataQualityMetricTypeDef

```python
# AnomalyDetectorDataQualityMetricTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyDetectorDataQualityMetricTypeDef


def get_value() -> AnomalyDetectorDataQualityMetricTypeDef:
    return {
        "StartTimestamp": ...,
    }


# AnomalyDetectorDataQualityMetricTypeDef definition

class AnomalyDetectorDataQualityMetricTypeDef(TypedDict):
    StartTimestamp: NotRequired[datetime],
    MetricSetDataQualityMetricList: NotRequired[List[MetricSetDataQualityMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricSetDataQualityMetricTypeDef](./type_defs.md#metricsetdataqualitymetrictypedef) 
## ContributionMatrixTypeDef

```python
# ContributionMatrixTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ContributionMatrixTypeDef


def get_value() -> ContributionMatrixTypeDef:
    return {
        "DimensionContributionList": ...,
    }


# ContributionMatrixTypeDef definition

class ContributionMatrixTypeDef(TypedDict):
    DimensionContributionList: NotRequired[List[DimensionContributionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionContributionTypeDef](./type_defs.md#dimensioncontributiontypedef) 
## ListAnomalyGroupTimeSeriesResponseTypeDef

```python
# ListAnomalyGroupTimeSeriesResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import ListAnomalyGroupTimeSeriesResponseTypeDef


def get_value() -> ListAnomalyGroupTimeSeriesResponseTypeDef:
    return {
        "AnomalyGroupId": ...,
    }


# ListAnomalyGroupTimeSeriesResponseTypeDef definition

class ListAnomalyGroupTimeSeriesResponseTypeDef(TypedDict):
    AnomalyGroupId: str,
    MetricName: str,
    TimestampList: List[str],
    TimeSeriesList: List[TimeSeriesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeSeriesTypeDef](./type_defs.md#timeseriestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3SourceConfigOutputTypeDef

```python
# S3SourceConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import S3SourceConfigOutputTypeDef


def get_value() -> S3SourceConfigOutputTypeDef:
    return {
        "RoleArn": ...,
    }


# S3SourceConfigOutputTypeDef definition

class S3SourceConfigOutputTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    TemplatedPathList: NotRequired[List[str]],
    HistoricalDataPathList: NotRequired[List[str]],
    FileFormatDescriptor: NotRequired[FileFormatDescriptorOutputTypeDef],  # (1)
```

1. See [:material-code-braces: FileFormatDescriptorOutputTypeDef](./type_defs.md#fileformatdescriptoroutputtypedef) 
## DescribeAlertResponseTypeDef

```python
# DescribeAlertResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeAlertResponseTypeDef


def get_value() -> DescribeAlertResponseTypeDef:
    return {
        "Alert": ...,
    }


# DescribeAlertResponseTypeDef definition

class DescribeAlertResponseTypeDef(TypedDict):
    Alert: AlertTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertTypeDef](./type_defs.md#alerttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAlertRequestTypeDef

```python
# CreateAlertRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CreateAlertRequestTypeDef


def get_value() -> CreateAlertRequestTypeDef:
    return {
        "AlertName": ...,
    }


# CreateAlertRequestTypeDef definition

class CreateAlertRequestTypeDef(TypedDict):
    AlertName: str,
    AnomalyDetectorArn: str,
    Action: ActionTypeDef,  # (1)
    AlertSensitivityThreshold: NotRequired[int],
    AlertDescription: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    AlertFilters: NotRequired[AlertFiltersUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) [:material-code-braces: AlertFiltersOutputTypeDef](./type_defs.md#alertfiltersoutputtypedef) 
## UpdateAlertRequestTypeDef

```python
# UpdateAlertRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import UpdateAlertRequestTypeDef


def get_value() -> UpdateAlertRequestTypeDef:
    return {
        "AlertArn": ...,
    }


# UpdateAlertRequestTypeDef definition

class UpdateAlertRequestTypeDef(TypedDict):
    AlertArn: str,
    AlertDescription: NotRequired[str],
    AlertSensitivityThreshold: NotRequired[int],
    Action: NotRequired[ActionTypeDef],  # (1)
    AlertFilters: NotRequired[AlertFiltersUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) [:material-code-braces: AlertFiltersOutputTypeDef](./type_defs.md#alertfiltersoutputtypedef) 
## DetectedFileFormatDescriptorTypeDef

```python
# DetectedFileFormatDescriptorTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectedFileFormatDescriptorTypeDef


def get_value() -> DetectedFileFormatDescriptorTypeDef:
    return {
        "CsvFormatDescriptor": ...,
    }


# DetectedFileFormatDescriptorTypeDef definition

class DetectedFileFormatDescriptorTypeDef(TypedDict):
    CsvFormatDescriptor: NotRequired[DetectedCsvFormatDescriptorTypeDef],  # (1)
    JsonFormatDescriptor: NotRequired[DetectedJsonFormatDescriptorTypeDef],  # (2)
```

1. See [:material-code-braces: DetectedCsvFormatDescriptorTypeDef](./type_defs.md#detectedcsvformatdescriptortypedef) 
2. See [:material-code-braces: DetectedJsonFormatDescriptorTypeDef](./type_defs.md#detectedjsonformatdescriptortypedef) 
## S3SourceConfigTypeDef

```python
# S3SourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import S3SourceConfigTypeDef


def get_value() -> S3SourceConfigTypeDef:
    return {
        "RoleArn": ...,
    }


# S3SourceConfigTypeDef definition

class S3SourceConfigTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    TemplatedPathList: NotRequired[Sequence[str]],
    HistoricalDataPathList: NotRequired[Sequence[str]],
    FileFormatDescriptor: NotRequired[FileFormatDescriptorTypeDef],  # (1)
```

1. See [:material-code-braces: FileFormatDescriptorTypeDef](./type_defs.md#fileformatdescriptortypedef) 
## GetDataQualityMetricsResponseTypeDef

```python
# GetDataQualityMetricsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetDataQualityMetricsResponseTypeDef


def get_value() -> GetDataQualityMetricsResponseTypeDef:
    return {
        "AnomalyDetectorDataQualityMetricList": ...,
    }


# GetDataQualityMetricsResponseTypeDef definition

class GetDataQualityMetricsResponseTypeDef(TypedDict):
    AnomalyDetectorDataQualityMetricList: List[AnomalyDetectorDataQualityMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyDetectorDataQualityMetricTypeDef](./type_defs.md#anomalydetectordataqualitymetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricLevelImpactTypeDef

```python
# MetricLevelImpactTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricLevelImpactTypeDef


def get_value() -> MetricLevelImpactTypeDef:
    return {
        "MetricName": ...,
    }


# MetricLevelImpactTypeDef definition

class MetricLevelImpactTypeDef(TypedDict):
    MetricName: NotRequired[str],
    NumTimeSeries: NotRequired[int],
    ContributionMatrix: NotRequired[ContributionMatrixTypeDef],  # (1)
```

1. See [:material-code-braces: ContributionMatrixTypeDef](./type_defs.md#contributionmatrixtypedef) 
## MetricSourceOutputTypeDef

```python
# MetricSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSourceOutputTypeDef


def get_value() -> MetricSourceOutputTypeDef:
    return {
        "S3SourceConfig": ...,
    }


# MetricSourceOutputTypeDef definition

class MetricSourceOutputTypeDef(TypedDict):
    S3SourceConfig: NotRequired[S3SourceConfigOutputTypeDef],  # (1)
    AppFlowConfig: NotRequired[AppFlowConfigTypeDef],  # (2)
    CloudWatchConfig: NotRequired[CloudWatchConfigTypeDef],  # (3)
    RDSSourceConfig: NotRequired[RDSSourceConfigOutputTypeDef],  # (4)
    RedshiftSourceConfig: NotRequired[RedshiftSourceConfigOutputTypeDef],  # (5)
    AthenaSourceConfig: NotRequired[AthenaSourceConfigTypeDef],  # (6)
```

1. See [:material-code-braces: S3SourceConfigOutputTypeDef](./type_defs.md#s3sourceconfigoutputtypedef) 
2. See [:material-code-braces: AppFlowConfigTypeDef](./type_defs.md#appflowconfigtypedef) 
3. See [:material-code-braces: CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef) 
4. See [:material-code-braces: RDSSourceConfigOutputTypeDef](./type_defs.md#rdssourceconfigoutputtypedef) 
5. See [:material-code-braces: RedshiftSourceConfigOutputTypeDef](./type_defs.md#redshiftsourceconfigoutputtypedef) 
6. See [:material-code-braces: AthenaSourceConfigTypeDef](./type_defs.md#athenasourceconfigtypedef) 
## DetectedS3SourceConfigTypeDef

```python
# DetectedS3SourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectedS3SourceConfigTypeDef


def get_value() -> DetectedS3SourceConfigTypeDef:
    return {
        "FileFormatDescriptor": ...,
    }


# DetectedS3SourceConfigTypeDef definition

class DetectedS3SourceConfigTypeDef(TypedDict):
    FileFormatDescriptor: NotRequired[DetectedFileFormatDescriptorTypeDef],  # (1)
```

1. See [:material-code-braces: DetectedFileFormatDescriptorTypeDef](./type_defs.md#detectedfileformatdescriptortypedef) 
## SampleDataS3SourceConfigTypeDef

```python
# SampleDataS3SourceConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import SampleDataS3SourceConfigTypeDef


def get_value() -> SampleDataS3SourceConfigTypeDef:
    return {
        "RoleArn": ...,
    }


# SampleDataS3SourceConfigTypeDef definition

class SampleDataS3SourceConfigTypeDef(TypedDict):
    RoleArn: str,
    FileFormatDescriptor: FileFormatDescriptorUnionTypeDef,  # (1)
    TemplatedPathList: NotRequired[Sequence[str]],
    HistoricalDataPathList: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: FileFormatDescriptorTypeDef](./type_defs.md#fileformatdescriptortypedef) [:material-code-braces: FileFormatDescriptorOutputTypeDef](./type_defs.md#fileformatdescriptoroutputtypedef) 
## MetricSourceTypeDef

```python
# MetricSourceTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import MetricSourceTypeDef


def get_value() -> MetricSourceTypeDef:
    return {
        "S3SourceConfig": ...,
    }


# MetricSourceTypeDef definition

class MetricSourceTypeDef(TypedDict):
    S3SourceConfig: NotRequired[S3SourceConfigTypeDef],  # (1)
    AppFlowConfig: NotRequired[AppFlowConfigTypeDef],  # (2)
    CloudWatchConfig: NotRequired[CloudWatchConfigTypeDef],  # (3)
    RDSSourceConfig: NotRequired[RDSSourceConfigTypeDef],  # (4)
    RedshiftSourceConfig: NotRequired[RedshiftSourceConfigTypeDef],  # (5)
    AthenaSourceConfig: NotRequired[AthenaSourceConfigTypeDef],  # (6)
```

1. See [:material-code-braces: S3SourceConfigTypeDef](./type_defs.md#s3sourceconfigtypedef) 
2. See [:material-code-braces: AppFlowConfigTypeDef](./type_defs.md#appflowconfigtypedef) 
3. See [:material-code-braces: CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef) 
4. See [:material-code-braces: RDSSourceConfigTypeDef](./type_defs.md#rdssourceconfigtypedef) 
5. See [:material-code-braces: RedshiftSourceConfigTypeDef](./type_defs.md#redshiftsourceconfigtypedef) 
6. See [:material-code-braces: AthenaSourceConfigTypeDef](./type_defs.md#athenasourceconfigtypedef) 
## AnomalyGroupTypeDef

```python
# AnomalyGroupTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import AnomalyGroupTypeDef


def get_value() -> AnomalyGroupTypeDef:
    return {
        "StartTime": ...,
    }


# AnomalyGroupTypeDef definition

class AnomalyGroupTypeDef(TypedDict):
    StartTime: NotRequired[str],
    EndTime: NotRequired[str],
    AnomalyGroupId: NotRequired[str],
    AnomalyGroupScore: NotRequired[float],
    PrimaryMetricName: NotRequired[str],
    MetricLevelImpactList: NotRequired[List[MetricLevelImpactTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricLevelImpactTypeDef](./type_defs.md#metriclevelimpacttypedef) 
## DescribeMetricSetResponseTypeDef

```python
# DescribeMetricSetResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DescribeMetricSetResponseTypeDef


def get_value() -> DescribeMetricSetResponseTypeDef:
    return {
        "MetricSetArn": ...,
    }


# DescribeMetricSetResponseTypeDef definition

class DescribeMetricSetResponseTypeDef(TypedDict):
    MetricSetArn: str,
    AnomalyDetectorArn: str,
    MetricSetName: str,
    MetricSetDescription: str,
    CreationTime: datetime,
    LastModificationTime: datetime,
    Offset: int,
    MetricList: List[MetricTypeDef],  # (1)
    TimestampColumn: TimestampColumnTypeDef,  # (2)
    DimensionList: List[str],
    MetricSetFrequency: FrequencyType,  # (3)
    Timezone: str,
    MetricSource: MetricSourceOutputTypeDef,  # (4)
    DimensionFilterList: List[MetricSetDimensionFilterOutputTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
3. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
4. See [:material-code-braces: MetricSourceOutputTypeDef](./type_defs.md#metricsourceoutputtypedef) 
5. See [:material-code-braces: MetricSetDimensionFilterOutputTypeDef](./type_defs.md#metricsetdimensionfilteroutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectedMetricSourceTypeDef

```python
# DetectedMetricSourceTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectedMetricSourceTypeDef


def get_value() -> DetectedMetricSourceTypeDef:
    return {
        "S3SourceConfig": ...,
    }


# DetectedMetricSourceTypeDef definition

class DetectedMetricSourceTypeDef(TypedDict):
    S3SourceConfig: NotRequired[DetectedS3SourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DetectedS3SourceConfigTypeDef](./type_defs.md#detecteds3sourceconfigtypedef) 
## GetSampleDataRequestTypeDef

```python
# GetSampleDataRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetSampleDataRequestTypeDef


def get_value() -> GetSampleDataRequestTypeDef:
    return {
        "S3SourceConfig": ...,
    }


# GetSampleDataRequestTypeDef definition

class GetSampleDataRequestTypeDef(TypedDict):
    S3SourceConfig: NotRequired[SampleDataS3SourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: SampleDataS3SourceConfigTypeDef](./type_defs.md#sampledatas3sourceconfigtypedef) 
## GetAnomalyGroupResponseTypeDef

```python
# GetAnomalyGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import GetAnomalyGroupResponseTypeDef


def get_value() -> GetAnomalyGroupResponseTypeDef:
    return {
        "AnomalyGroup": ...,
    }


# GetAnomalyGroupResponseTypeDef definition

class GetAnomalyGroupResponseTypeDef(TypedDict):
    AnomalyGroup: AnomalyGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyGroupTypeDef](./type_defs.md#anomalygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectedMetricSetConfigTypeDef

```python
# DetectedMetricSetConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectedMetricSetConfigTypeDef


def get_value() -> DetectedMetricSetConfigTypeDef:
    return {
        "Offset": ...,
    }


# DetectedMetricSetConfigTypeDef definition

class DetectedMetricSetConfigTypeDef(TypedDict):
    Offset: NotRequired[DetectedFieldTypeDef],  # (1)
    MetricSetFrequency: NotRequired[DetectedFieldTypeDef],  # (1)
    MetricSource: NotRequired[DetectedMetricSourceTypeDef],  # (3)
```

1. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
2. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
3. See [:material-code-braces: DetectedMetricSourceTypeDef](./type_defs.md#detectedmetricsourcetypedef) 
## CreateMetricSetRequestTypeDef

```python
# CreateMetricSetRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import CreateMetricSetRequestTypeDef


def get_value() -> CreateMetricSetRequestTypeDef:
    return {
        "AnomalyDetectorArn": ...,
    }


# CreateMetricSetRequestTypeDef definition

class CreateMetricSetRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    MetricSetName: str,
    MetricList: Sequence[MetricTypeDef],  # (1)
    MetricSource: MetricSourceUnionTypeDef,  # (2)
    MetricSetDescription: NotRequired[str],
    Offset: NotRequired[int],
    TimestampColumn: NotRequired[TimestampColumnTypeDef],  # (3)
    DimensionList: NotRequired[Sequence[str]],
    MetricSetFrequency: NotRequired[FrequencyType],  # (4)
    Timezone: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    DimensionFilterList: NotRequired[Sequence[MetricSetDimensionFilterUnionTypeDef]],  # (5)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) [:material-code-braces: MetricSourceOutputTypeDef](./type_defs.md#metricsourceoutputtypedef) 
3. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
4. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
5. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) [:material-code-braces: MetricSetDimensionFilterOutputTypeDef](./type_defs.md#metricsetdimensionfilteroutputtypedef) 
## UpdateMetricSetRequestTypeDef

```python
# UpdateMetricSetRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import UpdateMetricSetRequestTypeDef


def get_value() -> UpdateMetricSetRequestTypeDef:
    return {
        "MetricSetArn": ...,
    }


# UpdateMetricSetRequestTypeDef definition

class UpdateMetricSetRequestTypeDef(TypedDict):
    MetricSetArn: str,
    MetricSetDescription: NotRequired[str],
    MetricList: NotRequired[Sequence[MetricTypeDef]],  # (1)
    Offset: NotRequired[int],
    TimestampColumn: NotRequired[TimestampColumnTypeDef],  # (2)
    DimensionList: NotRequired[Sequence[str]],
    MetricSetFrequency: NotRequired[FrequencyType],  # (3)
    MetricSource: NotRequired[MetricSourceUnionTypeDef],  # (4)
    DimensionFilterList: NotRequired[Sequence[MetricSetDimensionFilterUnionTypeDef]],  # (5)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
3. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
4. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) [:material-code-braces: MetricSourceOutputTypeDef](./type_defs.md#metricsourceoutputtypedef) 
5. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) [:material-code-braces: MetricSetDimensionFilterOutputTypeDef](./type_defs.md#metricsetdimensionfilteroutputtypedef) 
## DetectMetricSetConfigResponseTypeDef

```python
# DetectMetricSetConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutmetrics.type_defs import DetectMetricSetConfigResponseTypeDef


def get_value() -> DetectMetricSetConfigResponseTypeDef:
    return {
        "DetectedMetricSetConfig": ...,
    }


# DetectMetricSetConfigResponseTypeDef definition

class DetectMetricSetConfigResponseTypeDef(TypedDict):
    DetectedMetricSetConfig: DetectedMetricSetConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectedMetricSetConfigTypeDef](./type_defs.md#detectedmetricsetconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
