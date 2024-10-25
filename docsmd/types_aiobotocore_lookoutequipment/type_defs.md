# Type definitions

> [Index](../README.md) > [LookoutEquipment](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LookoutEquipment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
    type annotations stubs module [types-aiobotocore-lookoutequipment](https://pypi.org/project/types-aiobotocore-lookoutequipment/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CategoricalValuesTypeDef

```python
# CategoricalValuesTypeDef definition

class CategoricalValuesTypeDef(TypedDict):
    Status: StatisticalIssueStatusType,  # (1)
    NumberOfCategory: NotRequired[int],
```

1. See [:material-code-brackets: StatisticalIssueStatusType](./literals.md#statisticalissuestatustype) 
## CountPercentTypeDef

```python
# CountPercentTypeDef definition

class CountPercentTypeDef(TypedDict):
    Count: int,
    Percentage: float,
```

## DatasetSchemaTypeDef

```python
# DatasetSchemaTypeDef definition

class DatasetSchemaTypeDef(TypedDict):
    InlineDataSchema: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DataPreProcessingConfigurationTypeDef

```python
# DataPreProcessingConfigurationTypeDef definition

class DataPreProcessingConfigurationTypeDef(TypedDict):
    TargetSamplingRate: NotRequired[TargetSamplingRateType],  # (1)
```

1. See [:material-code-brackets: TargetSamplingRateType](./literals.md#targetsamplingratetype) 
## DuplicateTimestampsTypeDef

```python
# DuplicateTimestampsTypeDef definition

class DuplicateTimestampsTypeDef(TypedDict):
    TotalNumberOfDuplicateTimestamps: int,
```

## InvalidSensorDataTypeDef

```python
# InvalidSensorDataTypeDef definition

class InvalidSensorDataTypeDef(TypedDict):
    AffectedSensorCount: int,
    TotalNumberOfInvalidValues: int,
```

## MissingSensorDataTypeDef

```python
# MissingSensorDataTypeDef definition

class MissingSensorDataTypeDef(TypedDict):
    AffectedSensorCount: int,
    TotalNumberOfMissingValues: int,
```

## UnsupportedTimestampsTypeDef

```python
# UnsupportedTimestampsTypeDef definition

class UnsupportedTimestampsTypeDef(TypedDict):
    TotalNumberOfUnsupportedTimestamps: int,
```

## DatasetSummaryTypeDef

```python
# DatasetSummaryTypeDef definition

class DatasetSummaryTypeDef(TypedDict):
    DatasetName: NotRequired[str],
    DatasetArn: NotRequired[str],
    Status: NotRequired[DatasetStatusType],  # (1)
    CreatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
## DeleteDatasetRequestRequestTypeDef

```python
# DeleteDatasetRequestRequestTypeDef definition

class DeleteDatasetRequestRequestTypeDef(TypedDict):
    DatasetName: str,
```

## DeleteInferenceSchedulerRequestRequestTypeDef

```python
# DeleteInferenceSchedulerRequestRequestTypeDef definition

class DeleteInferenceSchedulerRequestRequestTypeDef(TypedDict):
    InferenceSchedulerName: str,
```

## DeleteLabelGroupRequestRequestTypeDef

```python
# DeleteLabelGroupRequestRequestTypeDef definition

class DeleteLabelGroupRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
```

## DeleteLabelRequestRequestTypeDef

```python
# DeleteLabelRequestRequestTypeDef definition

class DeleteLabelRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
    LabelId: str,
```

## DeleteModelRequestRequestTypeDef

```python
# DeleteModelRequestRequestTypeDef definition

class DeleteModelRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeleteRetrainingSchedulerRequestRequestTypeDef

```python
# DeleteRetrainingSchedulerRequestRequestTypeDef definition

class DeleteRetrainingSchedulerRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## DescribeDataIngestionJobRequestRequestTypeDef

```python
# DescribeDataIngestionJobRequestRequestTypeDef definition

class DescribeDataIngestionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeDatasetRequestRequestTypeDef

```python
# DescribeDatasetRequestRequestTypeDef definition

class DescribeDatasetRequestRequestTypeDef(TypedDict):
    DatasetName: str,
```

## DescribeInferenceSchedulerRequestRequestTypeDef

```python
# DescribeInferenceSchedulerRequestRequestTypeDef definition

class DescribeInferenceSchedulerRequestRequestTypeDef(TypedDict):
    InferenceSchedulerName: str,
```

## DescribeLabelGroupRequestRequestTypeDef

```python
# DescribeLabelGroupRequestRequestTypeDef definition

class DescribeLabelGroupRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
```

## DescribeLabelRequestRequestTypeDef

```python
# DescribeLabelRequestRequestTypeDef definition

class DescribeLabelRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
    LabelId: str,
```

## DescribeModelRequestRequestTypeDef

```python
# DescribeModelRequestRequestTypeDef definition

class DescribeModelRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## DescribeModelVersionRequestRequestTypeDef

```python
# DescribeModelVersionRequestRequestTypeDef definition

class DescribeModelVersionRequestRequestTypeDef(TypedDict):
    ModelName: str,
    ModelVersion: int,
```

## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    Bucket: str,
    Key: str,
```

## DescribeResourcePolicyRequestRequestTypeDef

```python
# DescribeResourcePolicyRequestRequestTypeDef definition

class DescribeResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DescribeRetrainingSchedulerRequestRequestTypeDef

```python
# DescribeRetrainingSchedulerRequestRequestTypeDef definition

class DescribeRetrainingSchedulerRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## InferenceEventSummaryTypeDef

```python
# InferenceEventSummaryTypeDef definition

class InferenceEventSummaryTypeDef(TypedDict):
    InferenceSchedulerArn: NotRequired[str],
    InferenceSchedulerName: NotRequired[str],
    EventStartTime: NotRequired[datetime],
    EventEndTime: NotRequired[datetime],
    Diagnostics: NotRequired[str],
    EventDurationInSeconds: NotRequired[int],
```

## InferenceInputNameConfigurationTypeDef

```python
# InferenceInputNameConfigurationTypeDef definition

class InferenceInputNameConfigurationTypeDef(TypedDict):
    TimestampFormat: NotRequired[str],
    ComponentTimestampDelimiter: NotRequired[str],
```

## InferenceS3InputConfigurationTypeDef

```python
# InferenceS3InputConfigurationTypeDef definition

class InferenceS3InputConfigurationTypeDef(TypedDict):
    Bucket: str,
    Prefix: NotRequired[str],
```

## InferenceS3OutputConfigurationTypeDef

```python
# InferenceS3OutputConfigurationTypeDef definition

class InferenceS3OutputConfigurationTypeDef(TypedDict):
    Bucket: str,
    Prefix: NotRequired[str],
```

## InferenceSchedulerSummaryTypeDef

```python
# InferenceSchedulerSummaryTypeDef definition

class InferenceSchedulerSummaryTypeDef(TypedDict):
    ModelName: NotRequired[str],
    ModelArn: NotRequired[str],
    InferenceSchedulerName: NotRequired[str],
    InferenceSchedulerArn: NotRequired[str],
    Status: NotRequired[InferenceSchedulerStatusType],  # (1)
    DataDelayOffsetInMinutes: NotRequired[int],
    DataUploadFrequency: NotRequired[DataUploadFrequencyType],  # (2)
    LatestInferenceResult: NotRequired[LatestInferenceResultType],  # (3)
```

1. See [:material-code-brackets: InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype) 
2. See [:material-code-brackets: DataUploadFrequencyType](./literals.md#datauploadfrequencytype) 
3. See [:material-code-brackets: LatestInferenceResultType](./literals.md#latestinferenceresulttype) 
## IngestionS3InputConfigurationTypeDef

```python
# IngestionS3InputConfigurationTypeDef definition

class IngestionS3InputConfigurationTypeDef(TypedDict):
    Bucket: str,
    Prefix: NotRequired[str],
    KeyPattern: NotRequired[str],
```

## MissingCompleteSensorDataTypeDef

```python
# MissingCompleteSensorDataTypeDef definition

class MissingCompleteSensorDataTypeDef(TypedDict):
    AffectedSensorCount: int,
```

## SensorsWithShortDateRangeTypeDef

```python
# SensorsWithShortDateRangeTypeDef definition

class SensorsWithShortDateRangeTypeDef(TypedDict):
    AffectedSensorCount: int,
```

## LabelGroupSummaryTypeDef

```python
# LabelGroupSummaryTypeDef definition

class LabelGroupSummaryTypeDef(TypedDict):
    LabelGroupName: NotRequired[str],
    LabelGroupArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

## LabelSummaryTypeDef

```python
# LabelSummaryTypeDef definition

class LabelSummaryTypeDef(TypedDict):
    LabelGroupName: NotRequired[str],
    LabelId: NotRequired[str],
    LabelGroupArn: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Rating: NotRequired[LabelRatingType],  # (1)
    FaultCode: NotRequired[str],
    Equipment: NotRequired[str],
    CreatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: LabelRatingType](./literals.md#labelratingtype) 
## LabelsS3InputConfigurationTypeDef

```python
# LabelsS3InputConfigurationTypeDef definition

class LabelsS3InputConfigurationTypeDef(TypedDict):
    Bucket: str,
    Prefix: NotRequired[str],
```

## LargeTimestampGapsTypeDef

```python
# LargeTimestampGapsTypeDef definition

class LargeTimestampGapsTypeDef(TypedDict):
    Status: StatisticalIssueStatusType,  # (1)
    NumberOfLargeTimestampGaps: NotRequired[int],
    MaxTimestampGapInDays: NotRequired[int],
```

1. See [:material-code-brackets: StatisticalIssueStatusType](./literals.md#statisticalissuestatustype) 
## ListDataIngestionJobsRequestRequestTypeDef

```python
# ListDataIngestionJobsRequestRequestTypeDef definition

class ListDataIngestionJobsRequestRequestTypeDef(TypedDict):
    DatasetName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[IngestionJobStatusType],  # (1)
```

1. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
## ListDatasetsRequestRequestTypeDef

```python
# ListDatasetsRequestRequestTypeDef definition

class ListDatasetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    DatasetNameBeginsWith: NotRequired[str],
```

## ListInferenceSchedulersRequestRequestTypeDef

```python
# ListInferenceSchedulersRequestRequestTypeDef definition

class ListInferenceSchedulersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    InferenceSchedulerNameBeginsWith: NotRequired[str],
    ModelName: NotRequired[str],
    Status: NotRequired[InferenceSchedulerStatusType],  # (1)
```

1. See [:material-code-brackets: InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype) 
## ListLabelGroupsRequestRequestTypeDef

```python
# ListLabelGroupsRequestRequestTypeDef definition

class ListLabelGroupsRequestRequestTypeDef(TypedDict):
    LabelGroupNameBeginsWith: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ModelVersionSummaryTypeDef

```python
# ModelVersionSummaryTypeDef definition

class ModelVersionSummaryTypeDef(TypedDict):
    ModelName: NotRequired[str],
    ModelArn: NotRequired[str],
    ModelVersion: NotRequired[int],
    ModelVersionArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Status: NotRequired[ModelVersionStatusType],  # (1)
    SourceType: NotRequired[ModelVersionSourceTypeType],  # (2)
    ModelQuality: NotRequired[ModelQualityType],  # (3)
```

1. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
2. See [:material-code-brackets: ModelVersionSourceTypeType](./literals.md#modelversionsourcetypetype) 
3. See [:material-code-brackets: ModelQualityType](./literals.md#modelqualitytype) 
## ListModelsRequestRequestTypeDef

```python
# ListModelsRequestRequestTypeDef definition

class ListModelsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[ModelStatusType],  # (1)
    ModelNameBeginsWith: NotRequired[str],
    DatasetNameBeginsWith: NotRequired[str],
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
## ListRetrainingSchedulersRequestRequestTypeDef

```python
# ListRetrainingSchedulersRequestRequestTypeDef definition

class ListRetrainingSchedulersRequestRequestTypeDef(TypedDict):
    ModelNameBeginsWith: NotRequired[str],
    Status: NotRequired[RetrainingSchedulerStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
## RetrainingSchedulerSummaryTypeDef

```python
# RetrainingSchedulerSummaryTypeDef definition

class RetrainingSchedulerSummaryTypeDef(TypedDict):
    ModelName: NotRequired[str],
    ModelArn: NotRequired[str],
    Status: NotRequired[RetrainingSchedulerStatusType],  # (1)
    RetrainingStartDate: NotRequired[datetime],
    RetrainingFrequency: NotRequired[str],
    LookbackWindow: NotRequired[str],
```

1. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
## ListSensorStatisticsRequestRequestTypeDef

```python
# ListSensorStatisticsRequestRequestTypeDef definition

class ListSensorStatisticsRequestRequestTypeDef(TypedDict):
    DatasetName: str,
    IngestionJobId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ModelDiagnosticsS3OutputConfigurationTypeDef

```python
# ModelDiagnosticsS3OutputConfigurationTypeDef definition

class ModelDiagnosticsS3OutputConfigurationTypeDef(TypedDict):
    Bucket: str,
    Prefix: NotRequired[str],
```

## MonotonicValuesTypeDef

```python
# MonotonicValuesTypeDef definition

class MonotonicValuesTypeDef(TypedDict):
    Status: StatisticalIssueStatusType,  # (1)
    Monotonicity: NotRequired[MonotonicityType],  # (2)
```

1. See [:material-code-brackets: StatisticalIssueStatusType](./literals.md#statisticalissuestatustype) 
2. See [:material-code-brackets: MonotonicityType](./literals.md#monotonicitytype) 
## MultipleOperatingModesTypeDef

```python
# MultipleOperatingModesTypeDef definition

class MultipleOperatingModesTypeDef(TypedDict):
    Status: StatisticalIssueStatusType,  # (1)
```

1. See [:material-code-brackets: StatisticalIssueStatusType](./literals.md#statisticalissuestatustype) 
## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourcePolicy: str,
    ClientToken: str,
    PolicyRevisionId: NotRequired[str],
```

## StartInferenceSchedulerRequestRequestTypeDef

```python
# StartInferenceSchedulerRequestRequestTypeDef definition

class StartInferenceSchedulerRequestRequestTypeDef(TypedDict):
    InferenceSchedulerName: str,
```

## StartRetrainingSchedulerRequestRequestTypeDef

```python
# StartRetrainingSchedulerRequestRequestTypeDef definition

class StartRetrainingSchedulerRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## StopInferenceSchedulerRequestRequestTypeDef

```python
# StopInferenceSchedulerRequestRequestTypeDef definition

class StopInferenceSchedulerRequestRequestTypeDef(TypedDict):
    InferenceSchedulerName: str,
```

## StopRetrainingSchedulerRequestRequestTypeDef

```python
# StopRetrainingSchedulerRequestRequestTypeDef definition

class StopRetrainingSchedulerRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateActiveModelVersionRequestRequestTypeDef

```python
# UpdateActiveModelVersionRequestRequestTypeDef definition

class UpdateActiveModelVersionRequestRequestTypeDef(TypedDict):
    ModelName: str,
    ModelVersion: int,
```

## UpdateLabelGroupRequestRequestTypeDef

```python
# UpdateLabelGroupRequestRequestTypeDef definition

class UpdateLabelGroupRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
    FaultCodes: NotRequired[Sequence[str]],
```

## CreateDatasetRequestRequestTypeDef

```python
# CreateDatasetRequestRequestTypeDef definition

class CreateDatasetRequestRequestTypeDef(TypedDict):
    DatasetName: str,
    ClientToken: str,
    DatasetSchema: NotRequired[DatasetSchemaTypeDef],  # (1)
    ServerSideKmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DatasetSchemaTypeDef](./type_defs.md#datasetschematypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateLabelGroupRequestRequestTypeDef

```python
# CreateLabelGroupRequestRequestTypeDef definition

class CreateLabelGroupRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
    ClientToken: str,
    FaultCodes: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ImportDatasetRequestRequestTypeDef

```python
# ImportDatasetRequestRequestTypeDef definition

class ImportDatasetRequestRequestTypeDef(TypedDict):
    SourceDatasetArn: str,
    ClientToken: str,
    DatasetName: NotRequired[str],
    ServerSideKmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    DatasetName: str,
    DatasetArn: str,
    Status: DatasetStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInferenceSchedulerResponseTypeDef

```python
# CreateInferenceSchedulerResponseTypeDef definition

class CreateInferenceSchedulerResponseTypeDef(TypedDict):
    InferenceSchedulerArn: str,
    InferenceSchedulerName: str,
    Status: InferenceSchedulerStatusType,  # (1)
    ModelQuality: ModelQualityType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype) 
2. See [:material-code-brackets: ModelQualityType](./literals.md#modelqualitytype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLabelGroupResponseTypeDef

```python
# CreateLabelGroupResponseTypeDef definition

class CreateLabelGroupResponseTypeDef(TypedDict):
    LabelGroupName: str,
    LabelGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLabelResponseTypeDef

```python
# CreateLabelResponseTypeDef definition

class CreateLabelResponseTypeDef(TypedDict):
    LabelId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelResponseTypeDef

```python
# CreateModelResponseTypeDef definition

class CreateModelResponseTypeDef(TypedDict):
    ModelArn: str,
    Status: ModelStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRetrainingSchedulerResponseTypeDef

```python
# CreateRetrainingSchedulerResponseTypeDef definition

class CreateRetrainingSchedulerResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    Status: RetrainingSchedulerStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLabelGroupResponseTypeDef

```python
# DescribeLabelGroupResponseTypeDef definition

class DescribeLabelGroupResponseTypeDef(TypedDict):
    LabelGroupName: str,
    LabelGroupArn: str,
    FaultCodes: List[str],
    CreatedAt: datetime,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLabelResponseTypeDef

```python
# DescribeLabelResponseTypeDef definition

class DescribeLabelResponseTypeDef(TypedDict):
    LabelGroupName: str,
    LabelGroupArn: str,
    LabelId: str,
    StartTime: datetime,
    EndTime: datetime,
    Rating: LabelRatingType,  # (1)
    FaultCode: str,
    Notes: str,
    Equipment: str,
    CreatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LabelRatingType](./literals.md#labelratingtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourcePolicyResponseTypeDef

```python
# DescribeResourcePolicyResponseTypeDef definition

class DescribeResourcePolicyResponseTypeDef(TypedDict):
    PolicyRevisionId: str,
    ResourcePolicy: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRetrainingSchedulerResponseTypeDef

```python
# DescribeRetrainingSchedulerResponseTypeDef definition

class DescribeRetrainingSchedulerResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    RetrainingStartDate: datetime,
    RetrainingFrequency: str,
    LookbackWindow: str,
    Status: RetrainingSchedulerStatusType,  # (1)
    PromoteMode: ModelPromoteModeType,  # (2)
    CreatedAt: datetime,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
2. See [:material-code-brackets: ModelPromoteModeType](./literals.md#modelpromotemodetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportDatasetResponseTypeDef

```python
# ImportDatasetResponseTypeDef definition

class ImportDatasetResponseTypeDef(TypedDict):
    DatasetName: str,
    DatasetArn: str,
    Status: DatasetStatusType,  # (1)
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportModelVersionResponseTypeDef

```python
# ImportModelVersionResponseTypeDef definition

class ImportModelVersionResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    ModelVersionArn: str,
    ModelVersion: int,
    Status: ModelVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    ResourceArn: str,
    PolicyRevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataIngestionJobResponseTypeDef

```python
# StartDataIngestionJobResponseTypeDef definition

class StartDataIngestionJobResponseTypeDef(TypedDict):
    JobId: str,
    Status: IngestionJobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartInferenceSchedulerResponseTypeDef

```python
# StartInferenceSchedulerResponseTypeDef definition

class StartInferenceSchedulerResponseTypeDef(TypedDict):
    ModelArn: str,
    ModelName: str,
    InferenceSchedulerName: str,
    InferenceSchedulerArn: str,
    Status: InferenceSchedulerStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRetrainingSchedulerResponseTypeDef

```python
# StartRetrainingSchedulerResponseTypeDef definition

class StartRetrainingSchedulerResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    Status: RetrainingSchedulerStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopInferenceSchedulerResponseTypeDef

```python
# StopInferenceSchedulerResponseTypeDef definition

class StopInferenceSchedulerResponseTypeDef(TypedDict):
    ModelArn: str,
    ModelName: str,
    InferenceSchedulerName: str,
    InferenceSchedulerArn: str,
    Status: InferenceSchedulerStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopRetrainingSchedulerResponseTypeDef

```python
# StopRetrainingSchedulerResponseTypeDef definition

class StopRetrainingSchedulerResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    Status: RetrainingSchedulerStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateActiveModelVersionResponseTypeDef

```python
# UpdateActiveModelVersionResponseTypeDef definition

class UpdateActiveModelVersionResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    CurrentActiveVersion: int,
    PreviousActiveVersion: int,
    CurrentActiveVersionArn: str,
    PreviousActiveVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLabelRequestRequestTypeDef

```python
# CreateLabelRequestRequestTypeDef definition

class CreateLabelRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Rating: LabelRatingType,  # (1)
    ClientToken: str,
    FaultCode: NotRequired[str],
    Notes: NotRequired[str],
    Equipment: NotRequired[str],
```

1. See [:material-code-brackets: LabelRatingType](./literals.md#labelratingtype) 
## CreateRetrainingSchedulerRequestRequestTypeDef

```python
# CreateRetrainingSchedulerRequestRequestTypeDef definition

class CreateRetrainingSchedulerRequestRequestTypeDef(TypedDict):
    ModelName: str,
    RetrainingFrequency: str,
    LookbackWindow: str,
    ClientToken: str,
    RetrainingStartDate: NotRequired[TimestampTypeDef],
    PromoteMode: NotRequired[ModelPromoteModeType],  # (1)
```

1. See [:material-code-brackets: ModelPromoteModeType](./literals.md#modelpromotemodetype) 
## ListInferenceEventsRequestRequestTypeDef

```python
# ListInferenceEventsRequestRequestTypeDef definition

class ListInferenceEventsRequestRequestTypeDef(TypedDict):
    InferenceSchedulerName: str,
    IntervalStartTime: TimestampTypeDef,
    IntervalEndTime: TimestampTypeDef,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListInferenceExecutionsRequestRequestTypeDef

```python
# ListInferenceExecutionsRequestRequestTypeDef definition

class ListInferenceExecutionsRequestRequestTypeDef(TypedDict):
    InferenceSchedulerName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    DataStartTimeAfter: NotRequired[TimestampTypeDef],
    DataEndTimeBefore: NotRequired[TimestampTypeDef],
    Status: NotRequired[InferenceExecutionStatusType],  # (1)
```

1. See [:material-code-brackets: InferenceExecutionStatusType](./literals.md#inferenceexecutionstatustype) 
## ListLabelsRequestRequestTypeDef

```python
# ListLabelsRequestRequestTypeDef definition

class ListLabelsRequestRequestTypeDef(TypedDict):
    LabelGroupName: str,
    IntervalStartTime: NotRequired[TimestampTypeDef],
    IntervalEndTime: NotRequired[TimestampTypeDef],
    FaultCode: NotRequired[str],
    Equipment: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListModelVersionsRequestRequestTypeDef

```python
# ListModelVersionsRequestRequestTypeDef definition

class ListModelVersionsRequestRequestTypeDef(TypedDict):
    ModelName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[ModelVersionStatusType],  # (1)
    SourceType: NotRequired[ModelVersionSourceTypeType],  # (2)
    CreatedAtEndTime: NotRequired[TimestampTypeDef],
    CreatedAtStartTime: NotRequired[TimestampTypeDef],
    MaxModelVersion: NotRequired[int],
    MinModelVersion: NotRequired[int],
```

1. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
2. See [:material-code-brackets: ModelVersionSourceTypeType](./literals.md#modelversionsourcetypetype) 
## UpdateRetrainingSchedulerRequestRequestTypeDef

```python
# UpdateRetrainingSchedulerRequestRequestTypeDef definition

class UpdateRetrainingSchedulerRequestRequestTypeDef(TypedDict):
    ModelName: str,
    RetrainingStartDate: NotRequired[TimestampTypeDef],
    RetrainingFrequency: NotRequired[str],
    LookbackWindow: NotRequired[str],
    PromoteMode: NotRequired[ModelPromoteModeType],  # (1)
```

1. See [:material-code-brackets: ModelPromoteModeType](./literals.md#modelpromotemodetype) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef definition

class ListDatasetsResponseTypeDef(TypedDict):
    DatasetSummaries: List[DatasetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngestedFilesSummaryTypeDef

```python
# IngestedFilesSummaryTypeDef definition

class IngestedFilesSummaryTypeDef(TypedDict):
    TotalNumberOfFiles: int,
    IngestedNumberOfFiles: int,
    DiscardedFiles: NotRequired[List[S3ObjectTypeDef]],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## ListInferenceEventsResponseTypeDef

```python
# ListInferenceEventsResponseTypeDef definition

class ListInferenceEventsResponseTypeDef(TypedDict):
    InferenceEventSummaries: List[InferenceEventSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InferenceEventSummaryTypeDef](./type_defs.md#inferenceeventsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InferenceInputConfigurationTypeDef

```python
# InferenceInputConfigurationTypeDef definition

class InferenceInputConfigurationTypeDef(TypedDict):
    S3InputConfiguration: NotRequired[InferenceS3InputConfigurationTypeDef],  # (1)
    InputTimeZoneOffset: NotRequired[str],
    InferenceInputNameConfiguration: NotRequired[InferenceInputNameConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: InferenceS3InputConfigurationTypeDef](./type_defs.md#inferences3inputconfigurationtypedef) 
2. See [:material-code-braces: InferenceInputNameConfigurationTypeDef](./type_defs.md#inferenceinputnameconfigurationtypedef) 
## InferenceOutputConfigurationTypeDef

```python
# InferenceOutputConfigurationTypeDef definition

class InferenceOutputConfigurationTypeDef(TypedDict):
    S3OutputConfiguration: InferenceS3OutputConfigurationTypeDef,  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: InferenceS3OutputConfigurationTypeDef](./type_defs.md#inferences3outputconfigurationtypedef) 
## ListInferenceSchedulersResponseTypeDef

```python
# ListInferenceSchedulersResponseTypeDef definition

class ListInferenceSchedulersResponseTypeDef(TypedDict):
    InferenceSchedulerSummaries: List[InferenceSchedulerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InferenceSchedulerSummaryTypeDef](./type_defs.md#inferenceschedulersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngestionInputConfigurationTypeDef

```python
# IngestionInputConfigurationTypeDef definition

class IngestionInputConfigurationTypeDef(TypedDict):
    S3InputConfiguration: IngestionS3InputConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: IngestionS3InputConfigurationTypeDef](./type_defs.md#ingestions3inputconfigurationtypedef) 
## InsufficientSensorDataTypeDef

```python
# InsufficientSensorDataTypeDef definition

class InsufficientSensorDataTypeDef(TypedDict):
    MissingCompleteSensorData: MissingCompleteSensorDataTypeDef,  # (1)
    SensorsWithShortDateRange: SensorsWithShortDateRangeTypeDef,  # (2)
```

1. See [:material-code-braces: MissingCompleteSensorDataTypeDef](./type_defs.md#missingcompletesensordatatypedef) 
2. See [:material-code-braces: SensorsWithShortDateRangeTypeDef](./type_defs.md#sensorswithshortdaterangetypedef) 
## ListLabelGroupsResponseTypeDef

```python
# ListLabelGroupsResponseTypeDef definition

class ListLabelGroupsResponseTypeDef(TypedDict):
    LabelGroupSummaries: List[LabelGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LabelGroupSummaryTypeDef](./type_defs.md#labelgroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLabelsResponseTypeDef

```python
# ListLabelsResponseTypeDef definition

class ListLabelsResponseTypeDef(TypedDict):
    LabelSummaries: List[LabelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LabelSummaryTypeDef](./type_defs.md#labelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LabelsInputConfigurationTypeDef

```python
# LabelsInputConfigurationTypeDef definition

class LabelsInputConfigurationTypeDef(TypedDict):
    S3InputConfiguration: NotRequired[LabelsS3InputConfigurationTypeDef],  # (1)
    LabelGroupName: NotRequired[str],
```

1. See [:material-code-braces: LabelsS3InputConfigurationTypeDef](./type_defs.md#labelss3inputconfigurationtypedef) 
## ListModelVersionsResponseTypeDef

```python
# ListModelVersionsResponseTypeDef definition

class ListModelVersionsResponseTypeDef(TypedDict):
    ModelVersionSummaries: List[ModelVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelVersionSummaryTypeDef](./type_defs.md#modelversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRetrainingSchedulersResponseTypeDef

```python
# ListRetrainingSchedulersResponseTypeDef definition

class ListRetrainingSchedulersResponseTypeDef(TypedDict):
    RetrainingSchedulerSummaries: List[RetrainingSchedulerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RetrainingSchedulerSummaryTypeDef](./type_defs.md#retrainingschedulersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelDiagnosticsOutputConfigurationTypeDef

```python
# ModelDiagnosticsOutputConfigurationTypeDef definition

class ModelDiagnosticsOutputConfigurationTypeDef(TypedDict):
    S3OutputConfiguration: ModelDiagnosticsS3OutputConfigurationTypeDef,  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: ModelDiagnosticsS3OutputConfigurationTypeDef](./type_defs.md#modeldiagnosticss3outputconfigurationtypedef) 
## SensorStatisticsSummaryTypeDef

```python
# SensorStatisticsSummaryTypeDef definition

class SensorStatisticsSummaryTypeDef(TypedDict):
    ComponentName: NotRequired[str],
    SensorName: NotRequired[str],
    DataExists: NotRequired[bool],
    MissingValues: NotRequired[CountPercentTypeDef],  # (1)
    InvalidValues: NotRequired[CountPercentTypeDef],  # (1)
    InvalidDateEntries: NotRequired[CountPercentTypeDef],  # (1)
    DuplicateTimestamps: NotRequired[CountPercentTypeDef],  # (1)
    CategoricalValues: NotRequired[CategoricalValuesTypeDef],  # (5)
    MultipleOperatingModes: NotRequired[MultipleOperatingModesTypeDef],  # (6)
    LargeTimestampGaps: NotRequired[LargeTimestampGapsTypeDef],  # (7)
    MonotonicValues: NotRequired[MonotonicValuesTypeDef],  # (8)
    DataStartTime: NotRequired[datetime],
    DataEndTime: NotRequired[datetime],
```

1. See [:material-code-braces: CountPercentTypeDef](./type_defs.md#countpercenttypedef) 
2. See [:material-code-braces: CountPercentTypeDef](./type_defs.md#countpercenttypedef) 
3. See [:material-code-braces: CountPercentTypeDef](./type_defs.md#countpercenttypedef) 
4. See [:material-code-braces: CountPercentTypeDef](./type_defs.md#countpercenttypedef) 
5. See [:material-code-braces: CategoricalValuesTypeDef](./type_defs.md#categoricalvaluestypedef) 
6. See [:material-code-braces: MultipleOperatingModesTypeDef](./type_defs.md#multipleoperatingmodestypedef) 
7. See [:material-code-braces: LargeTimestampGapsTypeDef](./type_defs.md#largetimestampgapstypedef) 
8. See [:material-code-braces: MonotonicValuesTypeDef](./type_defs.md#monotonicvaluestypedef) 
## CreateInferenceSchedulerRequestRequestTypeDef

```python
# CreateInferenceSchedulerRequestRequestTypeDef definition

class CreateInferenceSchedulerRequestRequestTypeDef(TypedDict):
    ModelName: str,
    InferenceSchedulerName: str,
    DataUploadFrequency: DataUploadFrequencyType,  # (1)
    DataInputConfiguration: InferenceInputConfigurationTypeDef,  # (2)
    DataOutputConfiguration: InferenceOutputConfigurationTypeDef,  # (3)
    RoleArn: str,
    ClientToken: str,
    DataDelayOffsetInMinutes: NotRequired[int],
    ServerSideKmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: DataUploadFrequencyType](./literals.md#datauploadfrequencytype) 
2. See [:material-code-braces: InferenceInputConfigurationTypeDef](./type_defs.md#inferenceinputconfigurationtypedef) 
3. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeInferenceSchedulerResponseTypeDef

```python
# DescribeInferenceSchedulerResponseTypeDef definition

class DescribeInferenceSchedulerResponseTypeDef(TypedDict):
    ModelArn: str,
    ModelName: str,
    InferenceSchedulerName: str,
    InferenceSchedulerArn: str,
    Status: InferenceSchedulerStatusType,  # (1)
    DataDelayOffsetInMinutes: int,
    DataUploadFrequency: DataUploadFrequencyType,  # (2)
    CreatedAt: datetime,
    UpdatedAt: datetime,
    DataInputConfiguration: InferenceInputConfigurationTypeDef,  # (3)
    DataOutputConfiguration: InferenceOutputConfigurationTypeDef,  # (4)
    RoleArn: str,
    ServerSideKmsKeyId: str,
    LatestInferenceResult: LatestInferenceResultType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: InferenceSchedulerStatusType](./literals.md#inferenceschedulerstatustype) 
2. See [:material-code-brackets: DataUploadFrequencyType](./literals.md#datauploadfrequencytype) 
3. See [:material-code-braces: InferenceInputConfigurationTypeDef](./type_defs.md#inferenceinputconfigurationtypedef) 
4. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
5. See [:material-code-brackets: LatestInferenceResultType](./literals.md#latestinferenceresulttype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InferenceExecutionSummaryTypeDef

```python
# InferenceExecutionSummaryTypeDef definition

class InferenceExecutionSummaryTypeDef(TypedDict):
    ModelName: NotRequired[str],
    ModelArn: NotRequired[str],
    InferenceSchedulerName: NotRequired[str],
    InferenceSchedulerArn: NotRequired[str],
    ScheduledStartTime: NotRequired[datetime],
    DataStartTime: NotRequired[datetime],
    DataEndTime: NotRequired[datetime],
    DataInputConfiguration: NotRequired[InferenceInputConfigurationTypeDef],  # (1)
    DataOutputConfiguration: NotRequired[InferenceOutputConfigurationTypeDef],  # (2)
    CustomerResultObject: NotRequired[S3ObjectTypeDef],  # (3)
    Status: NotRequired[InferenceExecutionStatusType],  # (4)
    FailedReason: NotRequired[str],
    ModelVersion: NotRequired[int],
    ModelVersionArn: NotRequired[str],
```

1. See [:material-code-braces: InferenceInputConfigurationTypeDef](./type_defs.md#inferenceinputconfigurationtypedef) 
2. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
3. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
4. See [:material-code-brackets: InferenceExecutionStatusType](./literals.md#inferenceexecutionstatustype) 
## UpdateInferenceSchedulerRequestRequestTypeDef

```python
# UpdateInferenceSchedulerRequestRequestTypeDef definition

class UpdateInferenceSchedulerRequestRequestTypeDef(TypedDict):
    InferenceSchedulerName: str,
    DataDelayOffsetInMinutes: NotRequired[int],
    DataUploadFrequency: NotRequired[DataUploadFrequencyType],  # (1)
    DataInputConfiguration: NotRequired[InferenceInputConfigurationTypeDef],  # (2)
    DataOutputConfiguration: NotRequired[InferenceOutputConfigurationTypeDef],  # (3)
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: DataUploadFrequencyType](./literals.md#datauploadfrequencytype) 
2. See [:material-code-braces: InferenceInputConfigurationTypeDef](./type_defs.md#inferenceinputconfigurationtypedef) 
3. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
## DataIngestionJobSummaryTypeDef

```python
# DataIngestionJobSummaryTypeDef definition

class DataIngestionJobSummaryTypeDef(TypedDict):
    JobId: NotRequired[str],
    DatasetName: NotRequired[str],
    DatasetArn: NotRequired[str],
    IngestionInputConfiguration: NotRequired[IngestionInputConfigurationTypeDef],  # (1)
    Status: NotRequired[IngestionJobStatusType],  # (2)
```

1. See [:material-code-braces: IngestionInputConfigurationTypeDef](./type_defs.md#ingestioninputconfigurationtypedef) 
2. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
## StartDataIngestionJobRequestRequestTypeDef

```python
# StartDataIngestionJobRequestRequestTypeDef definition

class StartDataIngestionJobRequestRequestTypeDef(TypedDict):
    DatasetName: str,
    IngestionInputConfiguration: IngestionInputConfigurationTypeDef,  # (1)
    RoleArn: str,
    ClientToken: str,
```

1. See [:material-code-braces: IngestionInputConfigurationTypeDef](./type_defs.md#ingestioninputconfigurationtypedef) 
## DataQualitySummaryTypeDef

```python
# DataQualitySummaryTypeDef definition

class DataQualitySummaryTypeDef(TypedDict):
    InsufficientSensorData: InsufficientSensorDataTypeDef,  # (1)
    MissingSensorData: MissingSensorDataTypeDef,  # (2)
    InvalidSensorData: InvalidSensorDataTypeDef,  # (3)
    UnsupportedTimestamps: UnsupportedTimestampsTypeDef,  # (4)
    DuplicateTimestamps: DuplicateTimestampsTypeDef,  # (5)
```

1. See [:material-code-braces: InsufficientSensorDataTypeDef](./type_defs.md#insufficientsensordatatypedef) 
2. See [:material-code-braces: MissingSensorDataTypeDef](./type_defs.md#missingsensordatatypedef) 
3. See [:material-code-braces: InvalidSensorDataTypeDef](./type_defs.md#invalidsensordatatypedef) 
4. See [:material-code-braces: UnsupportedTimestampsTypeDef](./type_defs.md#unsupportedtimestampstypedef) 
5. See [:material-code-braces: DuplicateTimestampsTypeDef](./type_defs.md#duplicatetimestampstypedef) 
## ImportModelVersionRequestRequestTypeDef

```python
# ImportModelVersionRequestRequestTypeDef definition

class ImportModelVersionRequestRequestTypeDef(TypedDict):
    SourceModelVersionArn: str,
    DatasetName: str,
    ClientToken: str,
    ModelName: NotRequired[str],
    LabelsInputConfiguration: NotRequired[LabelsInputConfigurationTypeDef],  # (1)
    RoleArn: NotRequired[str],
    ServerSideKmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    InferenceDataImportStrategy: NotRequired[InferenceDataImportStrategyType],  # (3)
```

1. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: InferenceDataImportStrategyType](./literals.md#inferencedataimportstrategytype) 
## CreateModelRequestRequestTypeDef

```python
# CreateModelRequestRequestTypeDef definition

class CreateModelRequestRequestTypeDef(TypedDict):
    ModelName: str,
    DatasetName: str,
    ClientToken: str,
    DatasetSchema: NotRequired[DatasetSchemaTypeDef],  # (1)
    LabelsInputConfiguration: NotRequired[LabelsInputConfigurationTypeDef],  # (2)
    TrainingDataStartTime: NotRequired[TimestampTypeDef],
    TrainingDataEndTime: NotRequired[TimestampTypeDef],
    EvaluationDataStartTime: NotRequired[TimestampTypeDef],
    EvaluationDataEndTime: NotRequired[TimestampTypeDef],
    RoleArn: NotRequired[str],
    DataPreProcessingConfiguration: NotRequired[DataPreProcessingConfigurationTypeDef],  # (3)
    ServerSideKmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    OffCondition: NotRequired[str],
    ModelDiagnosticsOutputConfiguration: NotRequired[ModelDiagnosticsOutputConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: DatasetSchemaTypeDef](./type_defs.md#datasetschematypedef) 
2. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
3. See [:material-code-braces: DataPreProcessingConfigurationTypeDef](./type_defs.md#datapreprocessingconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef) 
## DescribeModelResponseTypeDef

```python
# DescribeModelResponseTypeDef definition

class DescribeModelResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    DatasetName: str,
    DatasetArn: str,
    Schema: str,
    LabelsInputConfiguration: LabelsInputConfigurationTypeDef,  # (1)
    TrainingDataStartTime: datetime,
    TrainingDataEndTime: datetime,
    EvaluationDataStartTime: datetime,
    EvaluationDataEndTime: datetime,
    RoleArn: str,
    DataPreProcessingConfiguration: DataPreProcessingConfigurationTypeDef,  # (2)
    Status: ModelStatusType,  # (3)
    TrainingExecutionStartTime: datetime,
    TrainingExecutionEndTime: datetime,
    FailedReason: str,
    ModelMetrics: str,
    LastUpdatedTime: datetime,
    CreatedAt: datetime,
    ServerSideKmsKeyId: str,
    OffCondition: str,
    SourceModelVersionArn: str,
    ImportJobStartTime: datetime,
    ImportJobEndTime: datetime,
    ActiveModelVersion: int,
    ActiveModelVersionArn: str,
    ModelVersionActivatedAt: datetime,
    PreviousActiveModelVersion: int,
    PreviousActiveModelVersionArn: str,
    PreviousModelVersionActivatedAt: datetime,
    PriorModelMetrics: str,
    LatestScheduledRetrainingFailedReason: str,
    LatestScheduledRetrainingStatus: ModelVersionStatusType,  # (4)
    LatestScheduledRetrainingModelVersion: int,
    LatestScheduledRetrainingStartTime: datetime,
    LatestScheduledRetrainingAvailableDataInDays: int,
    NextScheduledRetrainingStartDate: datetime,
    AccumulatedInferenceDataStartTime: datetime,
    AccumulatedInferenceDataEndTime: datetime,
    RetrainingSchedulerStatus: RetrainingSchedulerStatusType,  # (5)
    ModelDiagnosticsOutputConfiguration: ModelDiagnosticsOutputConfigurationTypeDef,  # (6)
    ModelQuality: ModelQualityType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
2. See [:material-code-braces: DataPreProcessingConfigurationTypeDef](./type_defs.md#datapreprocessingconfigurationtypedef) 
3. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
4. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
5. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
6. See [:material-code-braces: ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef) 
7. See [:material-code-brackets: ModelQualityType](./literals.md#modelqualitytype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeModelVersionResponseTypeDef

```python
# DescribeModelVersionResponseTypeDef definition

class DescribeModelVersionResponseTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    ModelVersion: int,
    ModelVersionArn: str,
    Status: ModelVersionStatusType,  # (1)
    SourceType: ModelVersionSourceTypeType,  # (2)
    DatasetName: str,
    DatasetArn: str,
    Schema: str,
    LabelsInputConfiguration: LabelsInputConfigurationTypeDef,  # (3)
    TrainingDataStartTime: datetime,
    TrainingDataEndTime: datetime,
    EvaluationDataStartTime: datetime,
    EvaluationDataEndTime: datetime,
    RoleArn: str,
    DataPreProcessingConfiguration: DataPreProcessingConfigurationTypeDef,  # (4)
    TrainingExecutionStartTime: datetime,
    TrainingExecutionEndTime: datetime,
    FailedReason: str,
    ModelMetrics: str,
    LastUpdatedTime: datetime,
    CreatedAt: datetime,
    ServerSideKmsKeyId: str,
    OffCondition: str,
    SourceModelVersionArn: str,
    ImportJobStartTime: datetime,
    ImportJobEndTime: datetime,
    ImportedDataSizeInBytes: int,
    PriorModelMetrics: str,
    RetrainingAvailableDataInDays: int,
    AutoPromotionResult: AutoPromotionResultType,  # (5)
    AutoPromotionResultReason: str,
    ModelDiagnosticsOutputConfiguration: ModelDiagnosticsOutputConfigurationTypeDef,  # (6)
    ModelDiagnosticsResultsObject: S3ObjectTypeDef,  # (7)
    ModelQuality: ModelQualityType,  # (8)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
2. See [:material-code-brackets: ModelVersionSourceTypeType](./literals.md#modelversionsourcetypetype) 
3. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
4. See [:material-code-braces: DataPreProcessingConfigurationTypeDef](./type_defs.md#datapreprocessingconfigurationtypedef) 
5. See [:material-code-brackets: AutoPromotionResultType](./literals.md#autopromotionresulttype) 
6. See [:material-code-braces: ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef) 
7. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
8. See [:material-code-brackets: ModelQualityType](./literals.md#modelqualitytype) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelSummaryTypeDef

```python
# ModelSummaryTypeDef definition

class ModelSummaryTypeDef(TypedDict):
    ModelName: NotRequired[str],
    ModelArn: NotRequired[str],
    DatasetName: NotRequired[str],
    DatasetArn: NotRequired[str],
    Status: NotRequired[ModelStatusType],  # (1)
    CreatedAt: NotRequired[datetime],
    ActiveModelVersion: NotRequired[int],
    ActiveModelVersionArn: NotRequired[str],
    LatestScheduledRetrainingStatus: NotRequired[ModelVersionStatusType],  # (2)
    LatestScheduledRetrainingModelVersion: NotRequired[int],
    LatestScheduledRetrainingStartTime: NotRequired[datetime],
    NextScheduledRetrainingStartDate: NotRequired[datetime],
    RetrainingSchedulerStatus: NotRequired[RetrainingSchedulerStatusType],  # (3)
    ModelDiagnosticsOutputConfiguration: NotRequired[ModelDiagnosticsOutputConfigurationTypeDef],  # (4)
    ModelQuality: NotRequired[ModelQualityType],  # (5)
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
2. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
3. See [:material-code-brackets: RetrainingSchedulerStatusType](./literals.md#retrainingschedulerstatustype) 
4. See [:material-code-braces: ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef) 
5. See [:material-code-brackets: ModelQualityType](./literals.md#modelqualitytype) 
## UpdateModelRequestRequestTypeDef

```python
# UpdateModelRequestRequestTypeDef definition

class UpdateModelRequestRequestTypeDef(TypedDict):
    ModelName: str,
    LabelsInputConfiguration: NotRequired[LabelsInputConfigurationTypeDef],  # (1)
    RoleArn: NotRequired[str],
    ModelDiagnosticsOutputConfiguration: NotRequired[ModelDiagnosticsOutputConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: LabelsInputConfigurationTypeDef](./type_defs.md#labelsinputconfigurationtypedef) 
2. See [:material-code-braces: ModelDiagnosticsOutputConfigurationTypeDef](./type_defs.md#modeldiagnosticsoutputconfigurationtypedef) 
## ListSensorStatisticsResponseTypeDef

```python
# ListSensorStatisticsResponseTypeDef definition

class ListSensorStatisticsResponseTypeDef(TypedDict):
    SensorStatisticsSummaries: List[SensorStatisticsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SensorStatisticsSummaryTypeDef](./type_defs.md#sensorstatisticssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInferenceExecutionsResponseTypeDef

```python
# ListInferenceExecutionsResponseTypeDef definition

class ListInferenceExecutionsResponseTypeDef(TypedDict):
    InferenceExecutionSummaries: List[InferenceExecutionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InferenceExecutionSummaryTypeDef](./type_defs.md#inferenceexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataIngestionJobsResponseTypeDef

```python
# ListDataIngestionJobsResponseTypeDef definition

class ListDataIngestionJobsResponseTypeDef(TypedDict):
    DataIngestionJobSummaries: List[DataIngestionJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataIngestionJobSummaryTypeDef](./type_defs.md#dataingestionjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataIngestionJobResponseTypeDef

```python
# DescribeDataIngestionJobResponseTypeDef definition

class DescribeDataIngestionJobResponseTypeDef(TypedDict):
    JobId: str,
    DatasetArn: str,
    IngestionInputConfiguration: IngestionInputConfigurationTypeDef,  # (1)
    RoleArn: str,
    CreatedAt: datetime,
    Status: IngestionJobStatusType,  # (2)
    FailedReason: str,
    DataQualitySummary: DataQualitySummaryTypeDef,  # (3)
    IngestedFilesSummary: IngestedFilesSummaryTypeDef,  # (4)
    StatusDetail: str,
    IngestedDataSize: int,
    DataStartTime: datetime,
    DataEndTime: datetime,
    SourceDatasetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IngestionInputConfigurationTypeDef](./type_defs.md#ingestioninputconfigurationtypedef) 
2. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
3. See [:material-code-braces: DataQualitySummaryTypeDef](./type_defs.md#dataqualitysummarytypedef) 
4. See [:material-code-braces: IngestedFilesSummaryTypeDef](./type_defs.md#ingestedfilessummarytypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    DatasetName: str,
    DatasetArn: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Status: DatasetStatusType,  # (1)
    Schema: str,
    ServerSideKmsKeyId: str,
    IngestionInputConfiguration: IngestionInputConfigurationTypeDef,  # (2)
    DataQualitySummary: DataQualitySummaryTypeDef,  # (3)
    IngestedFilesSummary: IngestedFilesSummaryTypeDef,  # (4)
    RoleArn: str,
    DataStartTime: datetime,
    DataEndTime: datetime,
    SourceDatasetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-braces: IngestionInputConfigurationTypeDef](./type_defs.md#ingestioninputconfigurationtypedef) 
3. See [:material-code-braces: DataQualitySummaryTypeDef](./type_defs.md#dataqualitysummarytypedef) 
4. See [:material-code-braces: IngestedFilesSummaryTypeDef](./type_defs.md#ingestedfilessummarytypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelsResponseTypeDef

```python
# ListModelsResponseTypeDef definition

class ListModelsResponseTypeDef(TypedDict):
    ModelSummaries: List[ModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelSummaryTypeDef](./type_defs.md#modelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
