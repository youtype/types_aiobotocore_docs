# Type definitions

> [Index](../README.md) > [LookoutMetrics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LookoutMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
    type annotations stubs module [types-aiobotocore-lookoutmetrics](https://pypi.org/project/types-aiobotocore-lookoutmetrics/).



## LambdaConfigurationTypeDef

```python
# LambdaConfigurationTypeDef definition

class LambdaConfigurationTypeDef(TypedDict):
    RoleArn: str,
    LambdaArn: str,
```

## SNSConfigurationTypeDef

```python
# SNSConfigurationTypeDef definition

class SNSConfigurationTypeDef(TypedDict):
    RoleArn: str,
    SnsTopicArn: str,
    SnsFormat: NotRequired[SnsFormatType],  # (1)
```

1. See [:material-code-brackets: SnsFormatType](./literals.md#snsformattype) 
## ActivateAnomalyDetectorRequestRequestTypeDef

```python
# ActivateAnomalyDetectorRequestRequestTypeDef definition

class ActivateAnomalyDetectorRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DimensionFilterTypeDef

```python
# DimensionFilterTypeDef definition

class DimensionFilterTypeDef(TypedDict):
    DimensionName: NotRequired[str],
    DimensionValueList: NotRequired[Sequence[str]],
```

## AlertSummaryTypeDef

```python
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
# AnomalyDetectorConfigSummaryTypeDef definition

class AnomalyDetectorConfigSummaryTypeDef(TypedDict):
    AnomalyDetectorFrequency: NotRequired[FrequencyType],  # (1)
```

1. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
## AnomalyDetectorConfigTypeDef

```python
# AnomalyDetectorConfigTypeDef definition

class AnomalyDetectorConfigTypeDef(TypedDict):
    AnomalyDetectorFrequency: NotRequired[FrequencyType],  # (1)
```

1. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
## AnomalyDetectorSummaryTypeDef

```python
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
# ItemizedMetricStatsTypeDef definition

class ItemizedMetricStatsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    OccurrenceCount: NotRequired[int],
```

## AnomalyGroupSummaryTypeDef

```python
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
# AnomalyGroupTimeSeriesFeedbackTypeDef definition

class AnomalyGroupTimeSeriesFeedbackTypeDef(TypedDict):
    AnomalyGroupId: str,
    TimeSeriesId: str,
    IsAnomaly: bool,
```

## AnomalyGroupTimeSeriesTypeDef

```python
# AnomalyGroupTimeSeriesTypeDef definition

class AnomalyGroupTimeSeriesTypeDef(TypedDict):
    AnomalyGroupId: str,
    TimeSeriesId: NotRequired[str],
```

## AppFlowConfigTypeDef

```python
# AppFlowConfigTypeDef definition

class AppFlowConfigTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    FlowName: NotRequired[str],
```

## BackTestConfigurationTypeDef

```python
# BackTestConfigurationTypeDef definition

class BackTestConfigurationTypeDef(TypedDict):
    RunBackTestMode: bool,
```

## AttributeValueTypeDef

```python
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
# AutoDetectionS3SourceConfigTypeDef definition

class AutoDetectionS3SourceConfigTypeDef(TypedDict):
    TemplatedPathList: NotRequired[Sequence[str]],
    HistoricalDataPathList: NotRequired[Sequence[str]],
```

## BackTestAnomalyDetectorRequestRequestTypeDef

```python
# BackTestAnomalyDetectorRequestRequestTypeDef definition

class BackTestAnomalyDetectorRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## MetricTypeDef

```python
# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    MetricName: str,
    AggregationFunction: AggregationFunctionType,  # (1)
    Namespace: NotRequired[str],
```

1. See [:material-code-brackets: AggregationFunctionType](./literals.md#aggregationfunctiontype) 
## TimestampColumnTypeDef

```python
# TimestampColumnTypeDef definition

class TimestampColumnTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    ColumnFormat: NotRequired[str],
```

## CsvFormatDescriptorTypeDef

```python
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
# DataQualityMetricTypeDef definition

class DataQualityMetricTypeDef(TypedDict):
    MetricType: NotRequired[DataQualityMetricTypeType],  # (1)
    MetricDescription: NotRequired[str],
    RelatedColumnName: NotRequired[str],
    MetricValue: NotRequired[float],
```

1. See [:material-code-brackets: DataQualityMetricTypeType](./literals.md#dataqualitymetrictypetype) 
## DeactivateAnomalyDetectorRequestRequestTypeDef

```python
# DeactivateAnomalyDetectorRequestRequestTypeDef definition

class DeactivateAnomalyDetectorRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DeleteAlertRequestRequestTypeDef

```python
# DeleteAlertRequestRequestTypeDef definition

class DeleteAlertRequestRequestTypeDef(TypedDict):
    AlertArn: str,
```

## DeleteAnomalyDetectorRequestRequestTypeDef

```python
# DeleteAnomalyDetectorRequestRequestTypeDef definition

class DeleteAnomalyDetectorRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DescribeAlertRequestRequestTypeDef

```python
# DescribeAlertRequestRequestTypeDef definition

class DescribeAlertRequestRequestTypeDef(TypedDict):
    AlertArn: str,
```

## DescribeAnomalyDetectionExecutionsRequestRequestTypeDef

```python
# DescribeAnomalyDetectionExecutionsRequestRequestTypeDef definition

class DescribeAnomalyDetectionExecutionsRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    Timestamp: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ExecutionStatusTypeDef

```python
# ExecutionStatusTypeDef definition

class ExecutionStatusTypeDef(TypedDict):
    Timestamp: NotRequired[str],
    Status: NotRequired[AnomalyDetectionTaskStatusType],  # (1)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: AnomalyDetectionTaskStatusType](./literals.md#anomalydetectiontaskstatustype) 
## DescribeAnomalyDetectorRequestRequestTypeDef

```python
# DescribeAnomalyDetectorRequestRequestTypeDef definition

class DescribeAnomalyDetectorRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
```

## DescribeMetricSetRequestRequestTypeDef

```python
# DescribeMetricSetRequestRequestTypeDef definition

class DescribeMetricSetRequestRequestTypeDef(TypedDict):
    MetricSetArn: str,
```

## DimensionValueContributionTypeDef

```python
# DimensionValueContributionTypeDef definition

class DimensionValueContributionTypeDef(TypedDict):
    DimensionValue: NotRequired[str],
    ContributionScore: NotRequired[float],
```

## DimensionNameValueTypeDef

```python
# DimensionNameValueTypeDef definition

class DimensionNameValueTypeDef(TypedDict):
    DimensionName: str,
    DimensionValue: str,
```

## JsonFormatDescriptorTypeDef

```python
# JsonFormatDescriptorTypeDef definition

class JsonFormatDescriptorTypeDef(TypedDict):
    FileCompression: NotRequired[JsonFileCompressionType],  # (1)
    Charset: NotRequired[str],
```

1. See [:material-code-brackets: JsonFileCompressionType](./literals.md#jsonfilecompressiontype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    DimensionValue: NotRequired[str],
    FilterOperation: NotRequired[FilterOperationType],  # (1)
```

1. See [:material-code-brackets: FilterOperationType](./literals.md#filteroperationtype) 
## GetAnomalyGroupRequestRequestTypeDef

```python
# GetAnomalyGroupRequestRequestTypeDef definition

class GetAnomalyGroupRequestRequestTypeDef(TypedDict):
    AnomalyGroupId: str,
    AnomalyDetectorArn: str,
```

## GetDataQualityMetricsRequestRequestTypeDef

```python
# GetDataQualityMetricsRequestRequestTypeDef definition

class GetDataQualityMetricsRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    MetricSetArn: NotRequired[str],
```

## TimeSeriesFeedbackTypeDef

```python
# TimeSeriesFeedbackTypeDef definition

class TimeSeriesFeedbackTypeDef(TypedDict):
    TimeSeriesId: NotRequired[str],
    IsAnomaly: NotRequired[bool],
```

## InterMetricImpactDetailsTypeDef

```python
# InterMetricImpactDetailsTypeDef definition

class InterMetricImpactDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    AnomalyGroupId: NotRequired[str],
    RelationshipType: NotRequired[RelationshipTypeType],  # (1)
    ContributionPercentage: NotRequired[float],
```

1. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
## ListAlertsRequestRequestTypeDef

```python
# ListAlertsRequestRequestTypeDef definition

class ListAlertsRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAnomalyDetectorsRequestRequestTypeDef

```python
# ListAnomalyDetectorsRequestRequestTypeDef definition

class ListAnomalyDetectorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAnomalyGroupRelatedMetricsRequestRequestTypeDef

```python
# ListAnomalyGroupRelatedMetricsRequestRequestTypeDef definition

class ListAnomalyGroupRelatedMetricsRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupId: str,
    RelationshipTypeFilter: NotRequired[RelationshipTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
## ListAnomalyGroupSummariesRequestRequestTypeDef

```python
# ListAnomalyGroupSummariesRequestRequestTypeDef definition

class ListAnomalyGroupSummariesRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    SensitivityThreshold: int,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAnomalyGroupTimeSeriesRequestRequestTypeDef

```python
# ListAnomalyGroupTimeSeriesRequestRequestTypeDef definition

class ListAnomalyGroupTimeSeriesRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupId: str,
    MetricName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMetricSetsRequestRequestTypeDef

```python
# ListMetricSetsRequestRequestTypeDef definition

class ListMetricSetsRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MetricSetSummaryTypeDef

```python
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

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    SubnetIdList: Sequence[str],
    SecurityGroupIdList: Sequence[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    SNSConfiguration: NotRequired[SNSConfigurationTypeDef],  # (1)
    LambdaConfiguration: NotRequired[LambdaConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: SNSConfigurationTypeDef](./type_defs.md#snsconfigurationtypedef) 
2. See [:material-code-braces: LambdaConfigurationTypeDef](./type_defs.md#lambdaconfigurationtypedef) 
## AlertFiltersTypeDef

```python
# AlertFiltersTypeDef definition

class AlertFiltersTypeDef(TypedDict):
    MetricList: NotRequired[Sequence[str]],
    DimensionFilterList: NotRequired[Sequence[DimensionFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef) 
## CreateAnomalyDetectorRequestRequestTypeDef

```python
# CreateAnomalyDetectorRequestRequestTypeDef definition

class CreateAnomalyDetectorRequestRequestTypeDef(TypedDict):
    AnomalyDetectorName: str,
    AnomalyDetectorConfig: AnomalyDetectorConfigTypeDef,  # (1)
    AnomalyDetectorDescription: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AnomalyDetectorConfigTypeDef](./type_defs.md#anomalydetectorconfigtypedef) 
## UpdateAnomalyDetectorRequestRequestTypeDef

```python
# UpdateAnomalyDetectorRequestRequestTypeDef definition

class UpdateAnomalyDetectorRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    KmsKeyArn: NotRequired[str],
    AnomalyDetectorDescription: NotRequired[str],
    AnomalyDetectorConfig: NotRequired[AnomalyDetectorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AnomalyDetectorConfigTypeDef](./type_defs.md#anomalydetectorconfigtypedef) 
## AnomalyGroupStatisticsTypeDef

```python
# AnomalyGroupStatisticsTypeDef definition

class AnomalyGroupStatisticsTypeDef(TypedDict):
    EvaluationStartDate: NotRequired[str],
    TotalCount: NotRequired[int],
    ItemizedMetricStatsList: NotRequired[List[ItemizedMetricStatsTypeDef]],  # (1)
```

1. See [:material-code-braces: ItemizedMetricStatsTypeDef](./type_defs.md#itemizedmetricstatstypedef) 
## PutFeedbackRequestRequestTypeDef

```python
# PutFeedbackRequestRequestTypeDef definition

class PutFeedbackRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesFeedbackTypeDef,  # (1)
```

1. See [:material-code-braces: AnomalyGroupTimeSeriesFeedbackTypeDef](./type_defs.md#anomalygrouptimeseriesfeedbacktypedef) 
## GetFeedbackRequestRequestTypeDef

```python
# GetFeedbackRequestRequestTypeDef definition

class GetFeedbackRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AnomalyGroupTimeSeriesFeedback: AnomalyGroupTimeSeriesTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnomalyGroupTimeSeriesTypeDef](./type_defs.md#anomalygrouptimeseriestypedef) 
## AthenaSourceConfigTypeDef

```python
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
# CloudWatchConfigTypeDef definition

class CloudWatchConfigTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    BackTestConfiguration: NotRequired[BackTestConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: BackTestConfigurationTypeDef](./type_defs.md#backtestconfigurationtypedef) 
## DetectedFieldTypeDef

```python
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
# AutoDetectionMetricSourceTypeDef definition

class AutoDetectionMetricSourceTypeDef(TypedDict):
    S3SourceConfig: NotRequired[AutoDetectionS3SourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AutoDetectionS3SourceConfigTypeDef](./type_defs.md#autodetections3sourceconfigtypedef) 
## CreateAlertResponseTypeDef

```python
# CreateAlertResponseTypeDef definition

class CreateAlertResponseTypeDef(TypedDict):
    AlertArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAnomalyDetectorResponseTypeDef

```python
# CreateAnomalyDetectorResponseTypeDef definition

class CreateAnomalyDetectorResponseTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMetricSetResponseTypeDef

```python
# CreateMetricSetResponseTypeDef definition

class CreateMetricSetResponseTypeDef(TypedDict):
    MetricSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAnomalyDetectorResponseTypeDef

```python
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
# GetSampleDataResponseTypeDef definition

class GetSampleDataResponseTypeDef(TypedDict):
    HeaderValues: List[str],
    SampleRows: List[List[str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlertsResponseTypeDef

```python
# ListAlertsResponseTypeDef definition

class ListAlertsResponseTypeDef(TypedDict):
    AlertSummaryList: List[AlertSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertSummaryTypeDef](./type_defs.md#alertsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnomalyDetectorsResponseTypeDef

```python
# ListAnomalyDetectorsResponseTypeDef definition

class ListAnomalyDetectorsResponseTypeDef(TypedDict):
    AnomalyDetectorSummaryList: List[AnomalyDetectorSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyDetectorSummaryTypeDef](./type_defs.md#anomalydetectorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAlertResponseTypeDef

```python
# UpdateAlertResponseTypeDef definition

class UpdateAlertResponseTypeDef(TypedDict):
    AlertArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnomalyDetectorResponseTypeDef

```python
# UpdateAnomalyDetectorResponseTypeDef definition

class UpdateAnomalyDetectorResponseTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMetricSetResponseTypeDef

```python
# UpdateMetricSetResponseTypeDef definition

class UpdateMetricSetResponseTypeDef(TypedDict):
    MetricSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricSetDataQualityMetricTypeDef

```python
# MetricSetDataQualityMetricTypeDef definition

class MetricSetDataQualityMetricTypeDef(TypedDict):
    MetricSetArn: NotRequired[str],
    DataQualityMetricList: NotRequired[List[DataQualityMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: DataQualityMetricTypeDef](./type_defs.md#dataqualitymetrictypedef) 
## DescribeAnomalyDetectionExecutionsResponseTypeDef

```python
# DescribeAnomalyDetectionExecutionsResponseTypeDef definition

class DescribeAnomalyDetectionExecutionsResponseTypeDef(TypedDict):
    ExecutionList: List[ExecutionStatusTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExecutionStatusTypeDef](./type_defs.md#executionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DimensionContributionTypeDef

```python
# DimensionContributionTypeDef definition

class DimensionContributionTypeDef(TypedDict):
    DimensionName: NotRequired[str],
    DimensionValueContributionList: NotRequired[List[DimensionValueContributionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionValueContributionTypeDef](./type_defs.md#dimensionvaluecontributiontypedef) 
## TimeSeriesTypeDef

```python
# TimeSeriesTypeDef definition

class TimeSeriesTypeDef(TypedDict):
    TimeSeriesId: str,
    DimensionList: List[DimensionNameValueTypeDef],  # (1)
    MetricValueList: List[float],
```

1. See [:material-code-braces: DimensionNameValueTypeDef](./type_defs.md#dimensionnamevaluetypedef) 
## FileFormatDescriptorTypeDef

```python
# FileFormatDescriptorTypeDef definition

class FileFormatDescriptorTypeDef(TypedDict):
    CsvFormatDescriptor: NotRequired[CsvFormatDescriptorTypeDef],  # (1)
    JsonFormatDescriptor: NotRequired[JsonFormatDescriptorTypeDef],  # (2)
```

1. See [:material-code-braces: CsvFormatDescriptorTypeDef](./type_defs.md#csvformatdescriptortypedef) 
2. See [:material-code-braces: JsonFormatDescriptorTypeDef](./type_defs.md#jsonformatdescriptortypedef) 
## MetricSetDimensionFilterTypeDef

```python
# MetricSetDimensionFilterTypeDef definition

class MetricSetDimensionFilterTypeDef(TypedDict):
    Name: NotRequired[str],
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetFeedbackResponseTypeDef

```python
# GetFeedbackResponseTypeDef definition

class GetFeedbackResponseTypeDef(TypedDict):
    AnomalyGroupTimeSeriesFeedback: List[TimeSeriesFeedbackTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeSeriesFeedbackTypeDef](./type_defs.md#timeseriesfeedbacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnomalyGroupRelatedMetricsResponseTypeDef

```python
# ListAnomalyGroupRelatedMetricsResponseTypeDef definition

class ListAnomalyGroupRelatedMetricsResponseTypeDef(TypedDict):
    InterMetricImpactList: List[InterMetricImpactDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InterMetricImpactDetailsTypeDef](./type_defs.md#intermetricimpactdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMetricSetsResponseTypeDef

```python
# ListMetricSetsResponseTypeDef definition

class ListMetricSetsResponseTypeDef(TypedDict):
    MetricSetSummaryList: List[MetricSetSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricSetSummaryTypeDef](./type_defs.md#metricsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RDSSourceConfigTypeDef

```python
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
    AlertFilters: NotRequired[AlertFiltersTypeDef],  # (4)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-brackets: AlertTypeType](./literals.md#alerttypetype) 
3. See [:material-code-brackets: AlertStatusType](./literals.md#alertstatustype) 
4. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) 
## CreateAlertRequestRequestTypeDef

```python
# CreateAlertRequestRequestTypeDef definition

class CreateAlertRequestRequestTypeDef(TypedDict):
    AlertName: str,
    AnomalyDetectorArn: str,
    Action: ActionTypeDef,  # (1)
    AlertSensitivityThreshold: NotRequired[int],
    AlertDescription: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    AlertFilters: NotRequired[AlertFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) 
## UpdateAlertRequestRequestTypeDef

```python
# UpdateAlertRequestRequestTypeDef definition

class UpdateAlertRequestRequestTypeDef(TypedDict):
    AlertArn: str,
    AlertDescription: NotRequired[str],
    AlertSensitivityThreshold: NotRequired[int],
    Action: NotRequired[ActionTypeDef],  # (1)
    AlertFilters: NotRequired[AlertFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: AlertFiltersTypeDef](./type_defs.md#alertfilterstypedef) 
## ListAnomalyGroupSummariesResponseTypeDef

```python
# ListAnomalyGroupSummariesResponseTypeDef definition

class ListAnomalyGroupSummariesResponseTypeDef(TypedDict):
    AnomalyGroupSummaryList: List[AnomalyGroupSummaryTypeDef],  # (1)
    AnomalyGroupStatistics: AnomalyGroupStatisticsTypeDef,  # (2)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AnomalyGroupSummaryTypeDef](./type_defs.md#anomalygroupsummarytypedef) 
2. See [:material-code-braces: AnomalyGroupStatisticsTypeDef](./type_defs.md#anomalygroupstatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectedCsvFormatDescriptorTypeDef

```python
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
# DetectedJsonFormatDescriptorTypeDef definition

class DetectedJsonFormatDescriptorTypeDef(TypedDict):
    FileCompression: NotRequired[DetectedFieldTypeDef],  # (1)
    Charset: NotRequired[DetectedFieldTypeDef],  # (1)
```

1. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
2. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
## DetectMetricSetConfigRequestRequestTypeDef

```python
# DetectMetricSetConfigRequestRequestTypeDef definition

class DetectMetricSetConfigRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    AutoDetectionMetricSource: AutoDetectionMetricSourceTypeDef,  # (1)
```

1. See [:material-code-braces: AutoDetectionMetricSourceTypeDef](./type_defs.md#autodetectionmetricsourcetypedef) 
## AnomalyDetectorDataQualityMetricTypeDef

```python
# AnomalyDetectorDataQualityMetricTypeDef definition

class AnomalyDetectorDataQualityMetricTypeDef(TypedDict):
    StartTimestamp: NotRequired[datetime],
    MetricSetDataQualityMetricList: NotRequired[List[MetricSetDataQualityMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricSetDataQualityMetricTypeDef](./type_defs.md#metricsetdataqualitymetrictypedef) 
## ContributionMatrixTypeDef

```python
# ContributionMatrixTypeDef definition

class ContributionMatrixTypeDef(TypedDict):
    DimensionContributionList: NotRequired[List[DimensionContributionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionContributionTypeDef](./type_defs.md#dimensioncontributiontypedef) 
## ListAnomalyGroupTimeSeriesResponseTypeDef

```python
# ListAnomalyGroupTimeSeriesResponseTypeDef definition

class ListAnomalyGroupTimeSeriesResponseTypeDef(TypedDict):
    AnomalyGroupId: str,
    MetricName: str,
    TimestampList: List[str],
    NextToken: str,
    TimeSeriesList: List[TimeSeriesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeSeriesTypeDef](./type_defs.md#timeseriestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3SourceConfigTypeDef

```python
# S3SourceConfigTypeDef definition

class S3SourceConfigTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    TemplatedPathList: NotRequired[Sequence[str]],
    HistoricalDataPathList: NotRequired[Sequence[str]],
    FileFormatDescriptor: NotRequired[FileFormatDescriptorTypeDef],  # (1)
```

1. See [:material-code-braces: FileFormatDescriptorTypeDef](./type_defs.md#fileformatdescriptortypedef) 
## SampleDataS3SourceConfigTypeDef

```python
# SampleDataS3SourceConfigTypeDef definition

class SampleDataS3SourceConfigTypeDef(TypedDict):
    RoleArn: str,
    FileFormatDescriptor: FileFormatDescriptorTypeDef,  # (1)
    TemplatedPathList: NotRequired[Sequence[str]],
    HistoricalDataPathList: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: FileFormatDescriptorTypeDef](./type_defs.md#fileformatdescriptortypedef) 
## DescribeAlertResponseTypeDef

```python
# DescribeAlertResponseTypeDef definition

class DescribeAlertResponseTypeDef(TypedDict):
    Alert: AlertTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertTypeDef](./type_defs.md#alerttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectedFileFormatDescriptorTypeDef

```python
# DetectedFileFormatDescriptorTypeDef definition

class DetectedFileFormatDescriptorTypeDef(TypedDict):
    CsvFormatDescriptor: NotRequired[DetectedCsvFormatDescriptorTypeDef],  # (1)
    JsonFormatDescriptor: NotRequired[DetectedJsonFormatDescriptorTypeDef],  # (2)
```

1. See [:material-code-braces: DetectedCsvFormatDescriptorTypeDef](./type_defs.md#detectedcsvformatdescriptortypedef) 
2. See [:material-code-braces: DetectedJsonFormatDescriptorTypeDef](./type_defs.md#detectedjsonformatdescriptortypedef) 
## GetDataQualityMetricsResponseTypeDef

```python
# GetDataQualityMetricsResponseTypeDef definition

class GetDataQualityMetricsResponseTypeDef(TypedDict):
    AnomalyDetectorDataQualityMetricList: List[AnomalyDetectorDataQualityMetricTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyDetectorDataQualityMetricTypeDef](./type_defs.md#anomalydetectordataqualitymetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricLevelImpactTypeDef

```python
# MetricLevelImpactTypeDef definition

class MetricLevelImpactTypeDef(TypedDict):
    MetricName: NotRequired[str],
    NumTimeSeries: NotRequired[int],
    ContributionMatrix: NotRequired[ContributionMatrixTypeDef],  # (1)
```

1. See [:material-code-braces: ContributionMatrixTypeDef](./type_defs.md#contributionmatrixtypedef) 
## MetricSourceTypeDef

```python
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
## GetSampleDataRequestRequestTypeDef

```python
# GetSampleDataRequestRequestTypeDef definition

class GetSampleDataRequestRequestTypeDef(TypedDict):
    S3SourceConfig: NotRequired[SampleDataS3SourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: SampleDataS3SourceConfigTypeDef](./type_defs.md#sampledatas3sourceconfigtypedef) 
## DetectedS3SourceConfigTypeDef

```python
# DetectedS3SourceConfigTypeDef definition

class DetectedS3SourceConfigTypeDef(TypedDict):
    FileFormatDescriptor: NotRequired[DetectedFileFormatDescriptorTypeDef],  # (1)
```

1. See [:material-code-braces: DetectedFileFormatDescriptorTypeDef](./type_defs.md#detectedfileformatdescriptortypedef) 
## AnomalyGroupTypeDef

```python
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
## CreateMetricSetRequestRequestTypeDef

```python
# CreateMetricSetRequestRequestTypeDef definition

class CreateMetricSetRequestRequestTypeDef(TypedDict):
    AnomalyDetectorArn: str,
    MetricSetName: str,
    MetricList: Sequence[MetricTypeDef],  # (1)
    MetricSource: MetricSourceTypeDef,  # (2)
    MetricSetDescription: NotRequired[str],
    Offset: NotRequired[int],
    TimestampColumn: NotRequired[TimestampColumnTypeDef],  # (3)
    DimensionList: NotRequired[Sequence[str]],
    MetricSetFrequency: NotRequired[FrequencyType],  # (4)
    Timezone: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    DimensionFilterList: NotRequired[Sequence[MetricSetDimensionFilterTypeDef]],  # (5)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) 
3. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
4. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
5. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) 
## DescribeMetricSetResponseTypeDef

```python
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
    MetricSource: MetricSourceTypeDef,  # (4)
    DimensionFilterList: List[MetricSetDimensionFilterTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
3. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
4. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) 
5. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMetricSetRequestRequestTypeDef

```python
# UpdateMetricSetRequestRequestTypeDef definition

class UpdateMetricSetRequestRequestTypeDef(TypedDict):
    MetricSetArn: str,
    MetricSetDescription: NotRequired[str],
    MetricList: NotRequired[Sequence[MetricTypeDef]],  # (1)
    Offset: NotRequired[int],
    TimestampColumn: NotRequired[TimestampColumnTypeDef],  # (2)
    DimensionList: NotRequired[Sequence[str]],
    MetricSetFrequency: NotRequired[FrequencyType],  # (3)
    MetricSource: NotRequired[MetricSourceTypeDef],  # (4)
    DimensionFilterList: NotRequired[Sequence[MetricSetDimensionFilterTypeDef]],  # (5)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: TimestampColumnTypeDef](./type_defs.md#timestampcolumntypedef) 
3. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
4. See [:material-code-braces: MetricSourceTypeDef](./type_defs.md#metricsourcetypedef) 
5. See [:material-code-braces: MetricSetDimensionFilterTypeDef](./type_defs.md#metricsetdimensionfiltertypedef) 
## DetectedMetricSourceTypeDef

```python
# DetectedMetricSourceTypeDef definition

class DetectedMetricSourceTypeDef(TypedDict):
    S3SourceConfig: NotRequired[DetectedS3SourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DetectedS3SourceConfigTypeDef](./type_defs.md#detecteds3sourceconfigtypedef) 
## GetAnomalyGroupResponseTypeDef

```python
# GetAnomalyGroupResponseTypeDef definition

class GetAnomalyGroupResponseTypeDef(TypedDict):
    AnomalyGroup: AnomalyGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyGroupTypeDef](./type_defs.md#anomalygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectedMetricSetConfigTypeDef

```python
# DetectedMetricSetConfigTypeDef definition

class DetectedMetricSetConfigTypeDef(TypedDict):
    Offset: NotRequired[DetectedFieldTypeDef],  # (1)
    MetricSetFrequency: NotRequired[DetectedFieldTypeDef],  # (1)
    MetricSource: NotRequired[DetectedMetricSourceTypeDef],  # (3)
```

1. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
2. See [:material-code-braces: DetectedFieldTypeDef](./type_defs.md#detectedfieldtypedef) 
3. See [:material-code-braces: DetectedMetricSourceTypeDef](./type_defs.md#detectedmetricsourcetypedef) 
## DetectMetricSetConfigResponseTypeDef

```python
# DetectMetricSetConfigResponseTypeDef definition

class DetectMetricSetConfigResponseTypeDef(TypedDict):
    DetectedMetricSetConfig: DetectedMetricSetConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectedMetricSetConfigTypeDef](./type_defs.md#detectedmetricsetconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
