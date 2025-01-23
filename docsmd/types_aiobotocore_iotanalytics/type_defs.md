# Type definitions

> [Index](../README.md) > [IoTAnalytics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AddAttributesActivityUnionTypeDef

```python
# AddAttributesActivityUnionTypeDef definition

AddAttributesActivityUnionTypeDef = Union[
    AddAttributesActivityTypeDef,  # (1)
    AddAttributesActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AddAttributesActivityTypeDef](./type_defs.md#addattributesactivitytypedef) 
2. See [:material-code-braces: AddAttributesActivityOutputTypeDef](./type_defs.md#addattributesactivityoutputtypedef) 

## RemoveAttributesActivityUnionTypeDef

```python
# RemoveAttributesActivityUnionTypeDef definition

RemoveAttributesActivityUnionTypeDef = Union[
    RemoveAttributesActivityTypeDef,  # (1)
    RemoveAttributesActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RemoveAttributesActivityTypeDef](./type_defs.md#removeattributesactivitytypedef) 
2. See [:material-code-braces: RemoveAttributesActivityOutputTypeDef](./type_defs.md#removeattributesactivityoutputtypedef) 

## SelectAttributesActivityUnionTypeDef

```python
# SelectAttributesActivityUnionTypeDef definition

SelectAttributesActivityUnionTypeDef = Union[
    SelectAttributesActivityTypeDef,  # (1)
    SelectAttributesActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SelectAttributesActivityTypeDef](./type_defs.md#selectattributesactivitytypedef) 
2. See [:material-code-braces: SelectAttributesActivityOutputTypeDef](./type_defs.md#selectattributesactivityoutputtypedef) 

## SchemaDefinitionUnionTypeDef

```python
# SchemaDefinitionUnionTypeDef definition

SchemaDefinitionUnionTypeDef = Union[
    SchemaDefinitionTypeDef,  # (1)
    SchemaDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
2. See [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 

## SqlQueryDatasetActionUnionTypeDef

```python
# SqlQueryDatasetActionUnionTypeDef definition

SqlQueryDatasetActionUnionTypeDef = Union[
    SqlQueryDatasetActionTypeDef,  # (1)
    SqlQueryDatasetActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SqlQueryDatasetActionTypeDef](./type_defs.md#sqlquerydatasetactiontypedef) 
2. See [:material-code-braces: SqlQueryDatasetActionOutputTypeDef](./type_defs.md#sqlquerydatasetactionoutputtypedef) 

## ContainerDatasetActionUnionTypeDef

```python
# ContainerDatasetActionUnionTypeDef definition

ContainerDatasetActionUnionTypeDef = Union[
    ContainerDatasetActionTypeDef,  # (1)
    ContainerDatasetActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContainerDatasetActionTypeDef](./type_defs.md#containerdatasetactiontypedef) 
2. See [:material-code-braces: ContainerDatasetActionOutputTypeDef](./type_defs.md#containerdatasetactionoutputtypedef) 

## PipelineActivityUnionTypeDef

```python
# PipelineActivityUnionTypeDef definition

PipelineActivityUnionTypeDef = Union[
    PipelineActivityTypeDef,  # (1)
    PipelineActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) 
2. See [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 

## ParquetConfigurationUnionTypeDef

```python
# ParquetConfigurationUnionTypeDef definition

ParquetConfigurationUnionTypeDef = Union[
    ParquetConfigurationTypeDef,  # (1)
    ParquetConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ParquetConfigurationTypeDef](./type_defs.md#parquetconfigurationtypedef) 
2. See [:material-code-braces: ParquetConfigurationOutputTypeDef](./type_defs.md#parquetconfigurationoutputtypedef) 

## DatasetActionUnionTypeDef

```python
# DatasetActionUnionTypeDef definition

DatasetActionUnionTypeDef = Union[
    DatasetActionTypeDef,  # (1)
    DatasetActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatasetActionTypeDef](./type_defs.md#datasetactiontypedef) 
2. See [:material-code-braces: DatasetActionOutputTypeDef](./type_defs.md#datasetactionoutputtypedef) 



## AddAttributesActivityOutputTypeDef

```python
# AddAttributesActivityOutputTypeDef definition

class AddAttributesActivityOutputTypeDef(TypedDict):
    name: str,
    attributes: Dict[str, str],
    next: NotRequired[str],
```

## AddAttributesActivityTypeDef

```python
# AddAttributesActivityTypeDef definition

class AddAttributesActivityTypeDef(TypedDict):
    name: str,
    attributes: Mapping[str, str],
    next: NotRequired[str],
```

## BatchPutMessageErrorEntryTypeDef

```python
# BatchPutMessageErrorEntryTypeDef definition

class BatchPutMessageErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
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

## CancelPipelineReprocessingRequestRequestTypeDef

```python
# CancelPipelineReprocessingRequestRequestTypeDef definition

class CancelPipelineReprocessingRequestRequestTypeDef(TypedDict):
    pipelineName: str,
    reprocessingId: str,
```

## ChannelActivityTypeDef

```python
# ChannelActivityTypeDef definition

class ChannelActivityTypeDef(TypedDict):
    name: str,
    channelName: str,
    next: NotRequired[str],
```

## ChannelMessagesTypeDef

```python
# ChannelMessagesTypeDef definition

class ChannelMessagesTypeDef(TypedDict):
    s3Paths: NotRequired[Sequence[str]],
```

## EstimatedResourceSizeTypeDef

```python
# EstimatedResourceSizeTypeDef definition

class EstimatedResourceSizeTypeDef(TypedDict):
    estimatedSizeInBytes: NotRequired[float],
    estimatedOn: NotRequired[datetime],
```

## CustomerManagedChannelS3StorageTypeDef

```python
# CustomerManagedChannelS3StorageTypeDef definition

class CustomerManagedChannelS3StorageTypeDef(TypedDict):
    bucket: str,
    roleArn: str,
    keyPrefix: NotRequired[str],
```

## CustomerManagedChannelS3StorageSummaryTypeDef

```python
# CustomerManagedChannelS3StorageSummaryTypeDef definition

class CustomerManagedChannelS3StorageSummaryTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
    roleArn: NotRequired[str],
```

## RetentionPeriodTypeDef

```python
# RetentionPeriodTypeDef definition

class RetentionPeriodTypeDef(TypedDict):
    unlimited: NotRequired[bool],
    numberOfDays: NotRequired[int],
```

## ColumnTypeDef

```python
# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    name: str,
    type: str,
```

## ResourceConfigurationTypeDef

```python
# ResourceConfigurationTypeDef definition

class ResourceConfigurationTypeDef(TypedDict):
    computeType: ComputeTypeType,  # (1)
    volumeSizeInGB: int,
```

1. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## CreateDatasetContentRequestRequestTypeDef

```python
# CreateDatasetContentRequestRequestTypeDef definition

class CreateDatasetContentRequestRequestTypeDef(TypedDict):
    datasetName: str,
    versionId: NotRequired[str],
```

## VersioningConfigurationTypeDef

```python
# VersioningConfigurationTypeDef definition

class VersioningConfigurationTypeDef(TypedDict):
    unlimited: NotRequired[bool],
    maxVersions: NotRequired[int],
```

## CustomerManagedDatastoreS3StorageSummaryTypeDef

```python
# CustomerManagedDatastoreS3StorageSummaryTypeDef definition

class CustomerManagedDatastoreS3StorageSummaryTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
    roleArn: NotRequired[str],
```

## CustomerManagedDatastoreS3StorageTypeDef

```python
# CustomerManagedDatastoreS3StorageTypeDef definition

class CustomerManagedDatastoreS3StorageTypeDef(TypedDict):
    bucket: str,
    roleArn: str,
    keyPrefix: NotRequired[str],
```

## DatasetActionSummaryTypeDef

```python
# DatasetActionSummaryTypeDef definition

class DatasetActionSummaryTypeDef(TypedDict):
    actionName: NotRequired[str],
    actionType: NotRequired[DatasetActionTypeType],  # (1)
```

1. See [:material-code-brackets: DatasetActionTypeType](./literals.md#datasetactiontypetype) 
## IotEventsDestinationConfigurationTypeDef

```python
# IotEventsDestinationConfigurationTypeDef definition

class IotEventsDestinationConfigurationTypeDef(TypedDict):
    inputName: str,
    roleArn: str,
```

## DatasetContentStatusTypeDef

```python
# DatasetContentStatusTypeDef definition

class DatasetContentStatusTypeDef(TypedDict):
    state: NotRequired[DatasetContentStateType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: DatasetContentStateType](./literals.md#datasetcontentstatetype) 
## DatasetContentVersionValueTypeDef

```python
# DatasetContentVersionValueTypeDef definition

class DatasetContentVersionValueTypeDef(TypedDict):
    datasetName: str,
```

## DatasetEntryTypeDef

```python
# DatasetEntryTypeDef definition

class DatasetEntryTypeDef(TypedDict):
    entryName: NotRequired[str],
    dataURI: NotRequired[str],
```

## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    expression: NotRequired[str],
```

## TriggeringDatasetTypeDef

```python
# TriggeringDatasetTypeDef definition

class TriggeringDatasetTypeDef(TypedDict):
    name: str,
```

## DatastoreActivityTypeDef

```python
# DatastoreActivityTypeDef definition

class DatastoreActivityTypeDef(TypedDict):
    name: str,
    datastoreName: str,
```

## IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef

```python
# IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef definition

class IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
```

## IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef

```python
# IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef definition

class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(TypedDict):
    bucket: str,
    keyPrefix: NotRequired[str],
```

## PartitionTypeDef

```python
# PartitionTypeDef definition

class PartitionTypeDef(TypedDict):
    attributeName: str,
```

## TimestampPartitionTypeDef

```python
# TimestampPartitionTypeDef definition

class TimestampPartitionTypeDef(TypedDict):
    attributeName: str,
    timestampFormat: NotRequired[str],
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    channelName: str,
```

## DeleteDatasetContentRequestRequestTypeDef

```python
# DeleteDatasetContentRequestRequestTypeDef definition

class DeleteDatasetContentRequestRequestTypeDef(TypedDict):
    datasetName: str,
    versionId: NotRequired[str],
```

## DeleteDatasetRequestRequestTypeDef

```python
# DeleteDatasetRequestRequestTypeDef definition

class DeleteDatasetRequestRequestTypeDef(TypedDict):
    datasetName: str,
```

## DeleteDatastoreRequestRequestTypeDef

```python
# DeleteDatastoreRequestRequestTypeDef definition

class DeleteDatastoreRequestRequestTypeDef(TypedDict):
    datastoreName: str,
```

## DeletePipelineRequestRequestTypeDef

```python
# DeletePipelineRequestRequestTypeDef definition

class DeletePipelineRequestRequestTypeDef(TypedDict):
    pipelineName: str,
```

## DeltaTimeSessionWindowConfigurationTypeDef

```python
# DeltaTimeSessionWindowConfigurationTypeDef definition

class DeltaTimeSessionWindowConfigurationTypeDef(TypedDict):
    timeoutInMinutes: int,
```

## DeltaTimeTypeDef

```python
# DeltaTimeTypeDef definition

class DeltaTimeTypeDef(TypedDict):
    offsetSeconds: int,
    timeExpression: str,
```

## DescribeChannelRequestRequestTypeDef

```python
# DescribeChannelRequestRequestTypeDef definition

class DescribeChannelRequestRequestTypeDef(TypedDict):
    channelName: str,
    includeStatistics: NotRequired[bool],
```

## DescribeDatasetRequestRequestTypeDef

```python
# DescribeDatasetRequestRequestTypeDef definition

class DescribeDatasetRequestRequestTypeDef(TypedDict):
    datasetName: str,
```

## DescribeDatastoreRequestRequestTypeDef

```python
# DescribeDatastoreRequestRequestTypeDef definition

class DescribeDatastoreRequestRequestTypeDef(TypedDict):
    datastoreName: str,
    includeStatistics: NotRequired[bool],
```

## LoggingOptionsTypeDef

```python
# LoggingOptionsTypeDef definition

class LoggingOptionsTypeDef(TypedDict):
    roleArn: str,
    level: LoggingLevelType,  # (1)
    enabled: bool,
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## DescribePipelineRequestRequestTypeDef

```python
# DescribePipelineRequestRequestTypeDef definition

class DescribePipelineRequestRequestTypeDef(TypedDict):
    pipelineName: str,
```

## DeviceRegistryEnrichActivityTypeDef

```python
# DeviceRegistryEnrichActivityTypeDef definition

class DeviceRegistryEnrichActivityTypeDef(TypedDict):
    name: str,
    attribute: str,
    thingName: str,
    roleArn: str,
    next: NotRequired[str],
```

## DeviceShadowEnrichActivityTypeDef

```python
# DeviceShadowEnrichActivityTypeDef definition

class DeviceShadowEnrichActivityTypeDef(TypedDict):
    name: str,
    attribute: str,
    thingName: str,
    roleArn: str,
    next: NotRequired[str],
```

## FilterActivityTypeDef

```python
# FilterActivityTypeDef definition

class FilterActivityTypeDef(TypedDict):
    name: str,
    filter: str,
    next: NotRequired[str],
```

## GetDatasetContentRequestRequestTypeDef

```python
# GetDatasetContentRequestRequestTypeDef definition

class GetDatasetContentRequestRequestTypeDef(TypedDict):
    datasetName: str,
    versionId: NotRequired[str],
```

## GlueConfigurationTypeDef

```python
# GlueConfigurationTypeDef definition

class GlueConfigurationTypeDef(TypedDict):
    tableName: str,
    databaseName: str,
```

## LambdaActivityTypeDef

```python
# LambdaActivityTypeDef definition

class LambdaActivityTypeDef(TypedDict):
    name: str,
    lambdaName: str,
    batchSize: int,
    next: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDatasetsRequestRequestTypeDef

```python
# ListDatasetsRequestRequestTypeDef definition

class ListDatasetsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDatastoresRequestRequestTypeDef

```python
# ListDatastoresRequestRequestTypeDef definition

class ListDatastoresRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPipelinesRequestRequestTypeDef

```python
# ListPipelinesRequestRequestTypeDef definition

class ListPipelinesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MathActivityTypeDef

```python
# MathActivityTypeDef definition

class MathActivityTypeDef(TypedDict):
    name: str,
    attribute: str,
    math: str,
    next: NotRequired[str],
```

## OutputFileUriValueTypeDef

```python
# OutputFileUriValueTypeDef definition

class OutputFileUriValueTypeDef(TypedDict):
    fileName: str,
```

## RemoveAttributesActivityOutputTypeDef

```python
# RemoveAttributesActivityOutputTypeDef definition

class RemoveAttributesActivityOutputTypeDef(TypedDict):
    name: str,
    attributes: List[str],
    next: NotRequired[str],
```

## SelectAttributesActivityOutputTypeDef

```python
# SelectAttributesActivityOutputTypeDef definition

class SelectAttributesActivityOutputTypeDef(TypedDict):
    name: str,
    attributes: List[str],
    next: NotRequired[str],
```

## ReprocessingSummaryTypeDef

```python
# ReprocessingSummaryTypeDef definition

class ReprocessingSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    status: NotRequired[ReprocessingStatusType],  # (1)
    creationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReprocessingStatusType](./literals.md#reprocessingstatustype) 
## RemoveAttributesActivityTypeDef

```python
# RemoveAttributesActivityTypeDef definition

class RemoveAttributesActivityTypeDef(TypedDict):
    name: str,
    attributes: Sequence[str],
    next: NotRequired[str],
```

## SelectAttributesActivityTypeDef

```python
# SelectAttributesActivityTypeDef definition

class SelectAttributesActivityTypeDef(TypedDict):
    name: str,
    attributes: Sequence[str],
    next: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## BatchPutMessageResponseTypeDef

```python
# BatchPutMessageResponseTypeDef definition

class BatchPutMessageResponseTypeDef(TypedDict):
    batchPutMessageErrorEntries: List[BatchPutMessageErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutMessageErrorEntryTypeDef](./type_defs.md#batchputmessageerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetContentResponseTypeDef

```python
# CreateDatasetContentResponseTypeDef definition

class CreateDatasetContentResponseTypeDef(TypedDict):
    versionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineResponseTypeDef

```python
# CreatePipelineResponseTypeDef definition

class CreatePipelineResponseTypeDef(TypedDict):
    pipelineName: str,
    pipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunPipelineActivityResponseTypeDef

```python
# RunPipelineActivityResponseTypeDef definition

class RunPipelineActivityResponseTypeDef(TypedDict):
    payloads: List[bytes],
    logResult: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SampleChannelDataResponseTypeDef

```python
# SampleChannelDataResponseTypeDef definition

class SampleChannelDataResponseTypeDef(TypedDict):
    payloads: List[bytes],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPipelineReprocessingResponseTypeDef

```python
# StartPipelineReprocessingResponseTypeDef definition

class StartPipelineReprocessingResponseTypeDef(TypedDict):
    reprocessingId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    messageId: str,
    payload: BlobTypeDef,
```

## ChannelStatisticsTypeDef

```python
# ChannelStatisticsTypeDef definition

class ChannelStatisticsTypeDef(TypedDict):
    size: NotRequired[EstimatedResourceSizeTypeDef],  # (1)
```

1. See [:material-code-braces: EstimatedResourceSizeTypeDef](./type_defs.md#estimatedresourcesizetypedef) 
## DatastoreStatisticsTypeDef

```python
# DatastoreStatisticsTypeDef definition

class DatastoreStatisticsTypeDef(TypedDict):
    size: NotRequired[EstimatedResourceSizeTypeDef],  # (1)
```

1. See [:material-code-braces: EstimatedResourceSizeTypeDef](./type_defs.md#estimatedresourcesizetypedef) 
## ChannelStorageOutputTypeDef

```python
# ChannelStorageOutputTypeDef definition

class ChannelStorageOutputTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Dict[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedChannelS3StorageTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerManagedChannelS3StorageTypeDef](./type_defs.md#customermanagedchannels3storagetypedef) 
## ChannelStorageTypeDef

```python
# ChannelStorageTypeDef definition

class ChannelStorageTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Mapping[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedChannelS3StorageTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerManagedChannelS3StorageTypeDef](./type_defs.md#customermanagedchannels3storagetypedef) 
## ChannelStorageSummaryTypeDef

```python
# ChannelStorageSummaryTypeDef definition

class ChannelStorageSummaryTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Dict[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedChannelS3StorageSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerManagedChannelS3StorageSummaryTypeDef](./type_defs.md#customermanagedchannels3storagesummarytypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    channelName: str,
    channelArn: str,
    retentionPeriod: RetentionPeriodTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    datasetName: str,
    datasetArn: str,
    retentionPeriod: RetentionPeriodTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatastoreResponseTypeDef

```python
# CreateDatastoreResponseTypeDef definition

class CreateDatastoreResponseTypeDef(TypedDict):
    datastoreName: str,
    datastoreArn: str,
    retentionPeriod: RetentionPeriodTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaDefinitionOutputTypeDef

```python
# SchemaDefinitionOutputTypeDef definition

class SchemaDefinitionOutputTypeDef(TypedDict):
    columns: NotRequired[List[ColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
## SchemaDefinitionTypeDef

```python
# SchemaDefinitionTypeDef definition

class SchemaDefinitionTypeDef(TypedDict):
    columns: NotRequired[Sequence[ColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DatasetContentSummaryTypeDef

```python
# DatasetContentSummaryTypeDef definition

class DatasetContentSummaryTypeDef(TypedDict):
    version: NotRequired[str],
    status: NotRequired[DatasetContentStatusTypeDef],  # (1)
    creationTime: NotRequired[datetime],
    scheduleTime: NotRequired[datetime],
    completionTime: NotRequired[datetime],
```

1. See [:material-code-braces: DatasetContentStatusTypeDef](./type_defs.md#datasetcontentstatustypedef) 
## GetDatasetContentResponseTypeDef

```python
# GetDatasetContentResponseTypeDef definition

class GetDatasetContentResponseTypeDef(TypedDict):
    entries: List[DatasetEntryTypeDef],  # (1)
    timestamp: datetime,
    status: DatasetContentStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DatasetEntryTypeDef](./type_defs.md#datasetentrytypedef) 
2. See [:material-code-braces: DatasetContentStatusTypeDef](./type_defs.md#datasetcontentstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetTriggerTypeDef

```python
# DatasetTriggerTypeDef definition

class DatasetTriggerTypeDef(TypedDict):
    schedule: NotRequired[ScheduleTypeDef],  # (1)
    dataset: NotRequired[TriggeringDatasetTypeDef],  # (2)
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: TriggeringDatasetTypeDef](./type_defs.md#triggeringdatasettypedef) 
## DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef

```python
# DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef definition

class DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef(TypedDict):
    customerManagedS3Storage: NotRequired[IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagesummarytypedef) 
## DatastoreIotSiteWiseMultiLayerStorageTypeDef

```python
# DatastoreIotSiteWiseMultiLayerStorageTypeDef definition

class DatastoreIotSiteWiseMultiLayerStorageTypeDef(TypedDict):
    customerManagedS3Storage: IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,  # (1)
```

1. See [:material-code-braces: IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagetypedef) 
## DatastorePartitionTypeDef

```python
# DatastorePartitionTypeDef definition

class DatastorePartitionTypeDef(TypedDict):
    attributePartition: NotRequired[PartitionTypeDef],  # (1)
    timestampPartition: NotRequired[TimestampPartitionTypeDef],  # (2)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: TimestampPartitionTypeDef](./type_defs.md#timestamppartitiontypedef) 
## LateDataRuleConfigurationTypeDef

```python
# LateDataRuleConfigurationTypeDef definition

class LateDataRuleConfigurationTypeDef(TypedDict):
    deltaTimeSessionWindowConfiguration: NotRequired[DeltaTimeSessionWindowConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DeltaTimeSessionWindowConfigurationTypeDef](./type_defs.md#deltatimesessionwindowconfigurationtypedef) 
## QueryFilterTypeDef

```python
# QueryFilterTypeDef definition

class QueryFilterTypeDef(TypedDict):
    deltaTime: NotRequired[DeltaTimeTypeDef],  # (1)
```

1. See [:material-code-braces: DeltaTimeTypeDef](./type_defs.md#deltatimetypedef) 
## DescribeLoggingOptionsResponseTypeDef

```python
# DescribeLoggingOptionsResponseTypeDef definition

class DescribeLoggingOptionsResponseTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingOptionsRequestRequestTypeDef

```python
# PutLoggingOptionsRequestRequestTypeDef definition

class PutLoggingOptionsRequestRequestTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    bucket: str,
    key: str,
    roleArn: str,
    glueConfiguration: NotRequired[GlueConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: GlueConfigurationTypeDef](./type_defs.md#glueconfigurationtypedef) 
## ListChannelsRequestPaginateTypeDef

```python
# ListChannelsRequestPaginateTypeDef definition

class ListChannelsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetsRequestPaginateTypeDef

```python
# ListDatasetsRequestPaginateTypeDef definition

class ListDatasetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatastoresRequestPaginateTypeDef

```python
# ListDatastoresRequestPaginateTypeDef definition

class ListDatastoresRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelinesRequestPaginateTypeDef

```python
# ListPipelinesRequestPaginateTypeDef definition

class ListPipelinesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetContentsRequestPaginateTypeDef

```python
# ListDatasetContentsRequestPaginateTypeDef definition

class ListDatasetContentsRequestPaginateTypeDef(TypedDict):
    datasetName: str,
    scheduledOnOrAfter: NotRequired[TimestampTypeDef],
    scheduledBefore: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetContentsRequestRequestTypeDef

```python
# ListDatasetContentsRequestRequestTypeDef definition

class ListDatasetContentsRequestRequestTypeDef(TypedDict):
    datasetName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    scheduledOnOrAfter: NotRequired[TimestampTypeDef],
    scheduledBefore: NotRequired[TimestampTypeDef],
```

## SampleChannelDataRequestRequestTypeDef

```python
# SampleChannelDataRequestRequestTypeDef definition

class SampleChannelDataRequestRequestTypeDef(TypedDict):
    channelName: str,
    maxMessages: NotRequired[int],
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
```

## StartPipelineReprocessingRequestRequestTypeDef

```python
# StartPipelineReprocessingRequestRequestTypeDef definition

class StartPipelineReprocessingRequestRequestTypeDef(TypedDict):
    pipelineName: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    channelMessages: NotRequired[ChannelMessagesTypeDef],  # (1)
```

1. See [:material-code-braces: ChannelMessagesTypeDef](./type_defs.md#channelmessagestypedef) 
## VariableTypeDef

```python
# VariableTypeDef definition

class VariableTypeDef(TypedDict):
    name: str,
    stringValue: NotRequired[str],
    doubleValue: NotRequired[float],
    datasetContentVersionValue: NotRequired[DatasetContentVersionValueTypeDef],  # (1)
    outputFileUriValue: NotRequired[OutputFileUriValueTypeDef],  # (2)
```

1. See [:material-code-braces: DatasetContentVersionValueTypeDef](./type_defs.md#datasetcontentversionvaluetypedef) 
2. See [:material-code-braces: OutputFileUriValueTypeDef](./type_defs.md#outputfileurivaluetypedef) 
## PipelineActivityOutputTypeDef

```python
# PipelineActivityOutputTypeDef definition

class PipelineActivityOutputTypeDef(TypedDict):
    channel: NotRequired[ChannelActivityTypeDef],  # (1)
    lambda: NotRequired[LambdaActivityTypeDef],  # (2)
    datastore: NotRequired[DatastoreActivityTypeDef],  # (3)
    addAttributes: NotRequired[AddAttributesActivityOutputTypeDef],  # (4)
    removeAttributes: NotRequired[RemoveAttributesActivityOutputTypeDef],  # (5)
    selectAttributes: NotRequired[SelectAttributesActivityOutputTypeDef],  # (6)
    filter: NotRequired[FilterActivityTypeDef],  # (7)
    math: NotRequired[MathActivityTypeDef],  # (8)
    deviceRegistryEnrich: NotRequired[DeviceRegistryEnrichActivityTypeDef],  # (9)
    deviceShadowEnrich: NotRequired[DeviceShadowEnrichActivityTypeDef],  # (10)
```

1. See [:material-code-braces: ChannelActivityTypeDef](./type_defs.md#channelactivitytypedef) 
2. See [:material-code-braces: LambdaActivityTypeDef](./type_defs.md#lambdaactivitytypedef) 
3. See [:material-code-braces: DatastoreActivityTypeDef](./type_defs.md#datastoreactivitytypedef) 
4. See [:material-code-braces: AddAttributesActivityOutputTypeDef](./type_defs.md#addattributesactivityoutputtypedef) 
5. See [:material-code-braces: RemoveAttributesActivityOutputTypeDef](./type_defs.md#removeattributesactivityoutputtypedef) 
6. See [:material-code-braces: SelectAttributesActivityOutputTypeDef](./type_defs.md#selectattributesactivityoutputtypedef) 
7. See [:material-code-braces: FilterActivityTypeDef](./type_defs.md#filteractivitytypedef) 
8. See [:material-code-braces: MathActivityTypeDef](./type_defs.md#mathactivitytypedef) 
9. See [:material-code-braces: DeviceRegistryEnrichActivityTypeDef](./type_defs.md#deviceregistryenrichactivitytypedef) 
10. See [:material-code-braces: DeviceShadowEnrichActivityTypeDef](./type_defs.md#deviceshadowenrichactivitytypedef) 
## PipelineSummaryTypeDef

```python
# PipelineSummaryTypeDef definition

class PipelineSummaryTypeDef(TypedDict):
    pipelineName: NotRequired[str],
    reprocessingSummaries: NotRequired[List[ReprocessingSummaryTypeDef]],  # (1)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-braces: ReprocessingSummaryTypeDef](./type_defs.md#reprocessingsummarytypedef) 
## BatchPutMessageRequestRequestTypeDef

```python
# BatchPutMessageRequestRequestTypeDef definition

class BatchPutMessageRequestRequestTypeDef(TypedDict):
    channelName: str,
    messages: Sequence[MessageTypeDef],  # (1)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    name: NotRequired[str],
    storage: NotRequired[ChannelStorageOutputTypeDef],  # (1)
    arn: NotRequired[str],
    status: NotRequired[ChannelStatusType],  # (2)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (3)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    lastMessageArrivalTime: NotRequired[datetime],
```

1. See [:material-code-braces: ChannelStorageOutputTypeDef](./type_defs.md#channelstorageoutputtypedef) 
2. See [:material-code-brackets: ChannelStatusType](./literals.md#channelstatustype) 
3. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    channelName: str,
    channelStorage: NotRequired[ChannelStorageTypeDef],  # (1)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    channelName: str,
    channelStorage: NotRequired[ChannelStorageTypeDef],  # (1)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
## ChannelSummaryTypeDef

```python
# ChannelSummaryTypeDef definition

class ChannelSummaryTypeDef(TypedDict):
    channelName: NotRequired[str],
    channelStorage: NotRequired[ChannelStorageSummaryTypeDef],  # (1)
    status: NotRequired[ChannelStatusType],  # (2)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    lastMessageArrivalTime: NotRequired[datetime],
```

1. See [:material-code-braces: ChannelStorageSummaryTypeDef](./type_defs.md#channelstoragesummarytypedef) 
2. See [:material-code-brackets: ChannelStatusType](./literals.md#channelstatustype) 
## ParquetConfigurationOutputTypeDef

```python
# ParquetConfigurationOutputTypeDef definition

class ParquetConfigurationOutputTypeDef(TypedDict):
    schemaDefinition: NotRequired[SchemaDefinitionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
## ListDatasetContentsResponseTypeDef

```python
# ListDatasetContentsResponseTypeDef definition

class ListDatasetContentsResponseTypeDef(TypedDict):
    datasetContentSummaries: List[DatasetContentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetContentSummaryTypeDef](./type_defs.md#datasetcontentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetSummaryTypeDef

```python
# DatasetSummaryTypeDef definition

class DatasetSummaryTypeDef(TypedDict):
    datasetName: NotRequired[str],
    status: NotRequired[DatasetStatusType],  # (1)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    triggers: NotRequired[List[DatasetTriggerTypeDef]],  # (2)
    actions: NotRequired[List[DatasetActionSummaryTypeDef]],  # (3)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-braces: DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef) 
3. See [:material-code-braces: DatasetActionSummaryTypeDef](./type_defs.md#datasetactionsummarytypedef) 
## DatastoreStorageSummaryTypeDef

```python
# DatastoreStorageSummaryTypeDef definition

class DatastoreStorageSummaryTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Dict[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedDatastoreS3StorageSummaryTypeDef],  # (1)
    iotSiteWiseMultiLayerStorage: NotRequired[DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerManagedDatastoreS3StorageSummaryTypeDef](./type_defs.md#customermanageddatastores3storagesummarytypedef) 
2. See [:material-code-braces: DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef](./type_defs.md#datastoreiotsitewisemultilayerstoragesummarytypedef) 
## DatastoreStorageOutputTypeDef

```python
# DatastoreStorageOutputTypeDef definition

class DatastoreStorageOutputTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Dict[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedDatastoreS3StorageTypeDef],  # (1)
    iotSiteWiseMultiLayerStorage: NotRequired[DatastoreIotSiteWiseMultiLayerStorageTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#customermanageddatastores3storagetypedef) 
2. See [:material-code-braces: DatastoreIotSiteWiseMultiLayerStorageTypeDef](./type_defs.md#datastoreiotsitewisemultilayerstoragetypedef) 
## DatastoreStorageTypeDef

```python
# DatastoreStorageTypeDef definition

class DatastoreStorageTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Mapping[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedDatastoreS3StorageTypeDef],  # (1)
    iotSiteWiseMultiLayerStorage: NotRequired[DatastoreIotSiteWiseMultiLayerStorageTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#customermanageddatastores3storagetypedef) 
2. See [:material-code-braces: DatastoreIotSiteWiseMultiLayerStorageTypeDef](./type_defs.md#datastoreiotsitewisemultilayerstoragetypedef) 
## DatastorePartitionsOutputTypeDef

```python
# DatastorePartitionsOutputTypeDef definition

class DatastorePartitionsOutputTypeDef(TypedDict):
    partitions: NotRequired[List[DatastorePartitionTypeDef]],  # (1)
```

1. See [:material-code-braces: DatastorePartitionTypeDef](./type_defs.md#datastorepartitiontypedef) 
## DatastorePartitionsTypeDef

```python
# DatastorePartitionsTypeDef definition

class DatastorePartitionsTypeDef(TypedDict):
    partitions: NotRequired[Sequence[DatastorePartitionTypeDef]],  # (1)
```

1. See [:material-code-braces: DatastorePartitionTypeDef](./type_defs.md#datastorepartitiontypedef) 
## LateDataRuleTypeDef

```python
# LateDataRuleTypeDef definition

class LateDataRuleTypeDef(TypedDict):
    ruleConfiguration: LateDataRuleConfigurationTypeDef,  # (1)
    ruleName: NotRequired[str],
```

1. See [:material-code-braces: LateDataRuleConfigurationTypeDef](./type_defs.md#latedataruleconfigurationtypedef) 
## SqlQueryDatasetActionOutputTypeDef

```python
# SqlQueryDatasetActionOutputTypeDef definition

class SqlQueryDatasetActionOutputTypeDef(TypedDict):
    sqlQuery: str,
    filters: NotRequired[List[QueryFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
## SqlQueryDatasetActionTypeDef

```python
# SqlQueryDatasetActionTypeDef definition

class SqlQueryDatasetActionTypeDef(TypedDict):
    sqlQuery: str,
    filters: NotRequired[Sequence[QueryFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
## DatasetContentDeliveryDestinationTypeDef

```python
# DatasetContentDeliveryDestinationTypeDef definition

class DatasetContentDeliveryDestinationTypeDef(TypedDict):
    iotEventsDestinationConfiguration: NotRequired[IotEventsDestinationConfigurationTypeDef],  # (1)
    s3DestinationConfiguration: NotRequired[S3DestinationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: IotEventsDestinationConfigurationTypeDef](./type_defs.md#ioteventsdestinationconfigurationtypedef) 
2. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## ContainerDatasetActionOutputTypeDef

```python
# ContainerDatasetActionOutputTypeDef definition

class ContainerDatasetActionOutputTypeDef(TypedDict):
    image: str,
    executionRoleArn: str,
    resourceConfiguration: ResourceConfigurationTypeDef,  # (1)
    variables: NotRequired[List[VariableTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourceConfigurationTypeDef](./type_defs.md#resourceconfigurationtypedef) 
2. See [:material-code-braces: VariableTypeDef](./type_defs.md#variabletypedef) 
## ContainerDatasetActionTypeDef

```python
# ContainerDatasetActionTypeDef definition

class ContainerDatasetActionTypeDef(TypedDict):
    image: str,
    executionRoleArn: str,
    resourceConfiguration: ResourceConfigurationTypeDef,  # (1)
    variables: NotRequired[Sequence[VariableTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourceConfigurationTypeDef](./type_defs.md#resourceconfigurationtypedef) 
2. See [:material-code-braces: VariableTypeDef](./type_defs.md#variabletypedef) 
## PipelineTypeDef

```python
# PipelineTypeDef definition

class PipelineTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    activities: NotRequired[List[PipelineActivityOutputTypeDef]],  # (1)
    reprocessingSummaries: NotRequired[List[ReprocessingSummaryTypeDef]],  # (2)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
2. See [:material-code-braces: ReprocessingSummaryTypeDef](./type_defs.md#reprocessingsummarytypedef) 
## ListPipelinesResponseTypeDef

```python
# ListPipelinesResponseTypeDef definition

class ListPipelinesResponseTypeDef(TypedDict):
    pipelineSummaries: List[PipelineSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PipelineActivityTypeDef

```python
# PipelineActivityTypeDef definition

class PipelineActivityTypeDef(TypedDict):
    channel: NotRequired[ChannelActivityTypeDef],  # (1)
    lambda: NotRequired[LambdaActivityTypeDef],  # (2)
    datastore: NotRequired[DatastoreActivityTypeDef],  # (3)
    addAttributes: NotRequired[AddAttributesActivityUnionTypeDef],  # (4)
    removeAttributes: NotRequired[RemoveAttributesActivityUnionTypeDef],  # (5)
    selectAttributes: NotRequired[SelectAttributesActivityUnionTypeDef],  # (6)
    filter: NotRequired[FilterActivityTypeDef],  # (7)
    math: NotRequired[MathActivityTypeDef],  # (8)
    deviceRegistryEnrich: NotRequired[DeviceRegistryEnrichActivityTypeDef],  # (9)
    deviceShadowEnrich: NotRequired[DeviceShadowEnrichActivityTypeDef],  # (10)
```

1. See [:material-code-braces: ChannelActivityTypeDef](./type_defs.md#channelactivitytypedef) 
2. See [:material-code-braces: LambdaActivityTypeDef](./type_defs.md#lambdaactivitytypedef) 
3. See [:material-code-braces: DatastoreActivityTypeDef](./type_defs.md#datastoreactivitytypedef) 
4. See [:material-code-braces: AddAttributesActivityTypeDef](./type_defs.md#addattributesactivitytypedef) [:material-code-braces: AddAttributesActivityOutputTypeDef](./type_defs.md#addattributesactivityoutputtypedef) 
5. See [:material-code-braces: RemoveAttributesActivityTypeDef](./type_defs.md#removeattributesactivitytypedef) [:material-code-braces: RemoveAttributesActivityOutputTypeDef](./type_defs.md#removeattributesactivityoutputtypedef) 
6. See [:material-code-braces: SelectAttributesActivityTypeDef](./type_defs.md#selectattributesactivitytypedef) [:material-code-braces: SelectAttributesActivityOutputTypeDef](./type_defs.md#selectattributesactivityoutputtypedef) 
7. See [:material-code-braces: FilterActivityTypeDef](./type_defs.md#filteractivitytypedef) 
8. See [:material-code-braces: MathActivityTypeDef](./type_defs.md#mathactivitytypedef) 
9. See [:material-code-braces: DeviceRegistryEnrichActivityTypeDef](./type_defs.md#deviceregistryenrichactivitytypedef) 
10. See [:material-code-braces: DeviceShadowEnrichActivityTypeDef](./type_defs.md#deviceshadowenrichactivitytypedef) 
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    statistics: ChannelStatisticsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ChannelStatisticsTypeDef](./type_defs.md#channelstatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    channelSummaries: List[ChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FileFormatConfigurationOutputTypeDef

```python
# FileFormatConfigurationOutputTypeDef definition

class FileFormatConfigurationOutputTypeDef(TypedDict):
    jsonConfiguration: NotRequired[Dict[str, Any]],
    parquetConfiguration: NotRequired[ParquetConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ParquetConfigurationOutputTypeDef](./type_defs.md#parquetconfigurationoutputtypedef) 
## ParquetConfigurationTypeDef

```python
# ParquetConfigurationTypeDef definition

class ParquetConfigurationTypeDef(TypedDict):
    schemaDefinition: NotRequired[SchemaDefinitionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef definition

class ListDatasetsResponseTypeDef(TypedDict):
    datasetSummaries: List[DatasetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatastoreSummaryTypeDef

```python
# DatastoreSummaryTypeDef definition

class DatastoreSummaryTypeDef(TypedDict):
    datastoreName: NotRequired[str],
    datastoreStorage: NotRequired[DatastoreStorageSummaryTypeDef],  # (1)
    status: NotRequired[DatastoreStatusType],  # (2)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    lastMessageArrivalTime: NotRequired[datetime],
    fileFormatType: NotRequired[FileFormatTypeType],  # (3)
    datastorePartitions: NotRequired[DatastorePartitionsOutputTypeDef],  # (4)
```

1. See [:material-code-braces: DatastoreStorageSummaryTypeDef](./type_defs.md#datastorestoragesummarytypedef) 
2. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
3. See [:material-code-brackets: FileFormatTypeType](./literals.md#fileformattypetype) 
4. See [:material-code-braces: DatastorePartitionsOutputTypeDef](./type_defs.md#datastorepartitionsoutputtypedef) 
## DatasetContentDeliveryRuleTypeDef

```python
# DatasetContentDeliveryRuleTypeDef definition

class DatasetContentDeliveryRuleTypeDef(TypedDict):
    destination: DatasetContentDeliveryDestinationTypeDef,  # (1)
    entryName: NotRequired[str],
```

1. See [:material-code-braces: DatasetContentDeliveryDestinationTypeDef](./type_defs.md#datasetcontentdeliverydestinationtypedef) 
## DatasetActionOutputTypeDef

```python
# DatasetActionOutputTypeDef definition

class DatasetActionOutputTypeDef(TypedDict):
    actionName: NotRequired[str],
    queryAction: NotRequired[SqlQueryDatasetActionOutputTypeDef],  # (1)
    containerAction: NotRequired[ContainerDatasetActionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: SqlQueryDatasetActionOutputTypeDef](./type_defs.md#sqlquerydatasetactionoutputtypedef) 
2. See [:material-code-braces: ContainerDatasetActionOutputTypeDef](./type_defs.md#containerdatasetactionoutputtypedef) 
## DescribePipelineResponseTypeDef

```python
# DescribePipelineResponseTypeDef definition

class DescribePipelineResponseTypeDef(TypedDict):
    pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunPipelineActivityRequestRequestTypeDef

```python
# RunPipelineActivityRequestRequestTypeDef definition

class RunPipelineActivityRequestRequestTypeDef(TypedDict):
    pipelineActivity: PipelineActivityTypeDef,  # (1)
    payloads: Sequence[BlobTypeDef],
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) 
## UpdatePipelineRequestRequestTypeDef

```python
# UpdatePipelineRequestRequestTypeDef definition

class UpdatePipelineRequestRequestTypeDef(TypedDict):
    pipelineName: str,
    pipelineActivities: Sequence[PipelineActivityTypeDef],  # (1)
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) 
## DatastoreTypeDef

```python
# DatastoreTypeDef definition

class DatastoreTypeDef(TypedDict):
    name: NotRequired[str],
    storage: NotRequired[DatastoreStorageOutputTypeDef],  # (1)
    arn: NotRequired[str],
    status: NotRequired[DatastoreStatusType],  # (2)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (3)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    lastMessageArrivalTime: NotRequired[datetime],
    fileFormatConfiguration: NotRequired[FileFormatConfigurationOutputTypeDef],  # (4)
    datastorePartitions: NotRequired[DatastorePartitionsOutputTypeDef],  # (5)
```

1. See [:material-code-braces: DatastoreStorageOutputTypeDef](./type_defs.md#datastorestorageoutputtypedef) 
2. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
3. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
4. See [:material-code-braces: FileFormatConfigurationOutputTypeDef](./type_defs.md#fileformatconfigurationoutputtypedef) 
5. See [:material-code-braces: DatastorePartitionsOutputTypeDef](./type_defs.md#datastorepartitionsoutputtypedef) 
## ListDatastoresResponseTypeDef

```python
# ListDatastoresResponseTypeDef definition

class ListDatastoresResponseTypeDef(TypedDict):
    datastoreSummaries: List[DatastoreSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DatastoreSummaryTypeDef](./type_defs.md#datastoresummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetTypeDef

```python
# DatasetTypeDef definition

class DatasetTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    actions: NotRequired[List[DatasetActionOutputTypeDef]],  # (1)
    triggers: NotRequired[List[DatasetTriggerTypeDef]],  # (2)
    contentDeliveryRules: NotRequired[List[DatasetContentDeliveryRuleTypeDef]],  # (3)
    status: NotRequired[DatasetStatusType],  # (4)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (5)
    versioningConfiguration: NotRequired[VersioningConfigurationTypeDef],  # (6)
    lateDataRules: NotRequired[List[LateDataRuleTypeDef]],  # (7)
```

1. See [:material-code-braces: DatasetActionOutputTypeDef](./type_defs.md#datasetactionoutputtypedef) 
2. See [:material-code-braces: DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef) 
3. See [:material-code-braces: DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef) 
4. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
5. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
6. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
7. See [:material-code-braces: LateDataRuleTypeDef](./type_defs.md#latedataruletypedef) 
## DatasetActionTypeDef

```python
# DatasetActionTypeDef definition

class DatasetActionTypeDef(TypedDict):
    actionName: NotRequired[str],
    queryAction: NotRequired[SqlQueryDatasetActionUnionTypeDef],  # (1)
    containerAction: NotRequired[ContainerDatasetActionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: SqlQueryDatasetActionTypeDef](./type_defs.md#sqlquerydatasetactiontypedef) [:material-code-braces: SqlQueryDatasetActionOutputTypeDef](./type_defs.md#sqlquerydatasetactionoutputtypedef) 
2. See [:material-code-braces: ContainerDatasetActionTypeDef](./type_defs.md#containerdatasetactiontypedef) [:material-code-braces: ContainerDatasetActionOutputTypeDef](./type_defs.md#containerdatasetactionoutputtypedef) 
## CreatePipelineRequestRequestTypeDef

```python
# CreatePipelineRequestRequestTypeDef definition

class CreatePipelineRequestRequestTypeDef(TypedDict):
    pipelineName: str,
    pipelineActivities: Sequence[PipelineActivityUnionTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeDatastoreResponseTypeDef

```python
# DescribeDatastoreResponseTypeDef definition

class DescribeDatastoreResponseTypeDef(TypedDict):
    datastore: DatastoreTypeDef,  # (1)
    statistics: DatastoreStatisticsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DatastoreTypeDef](./type_defs.md#datastoretypedef) 
2. See [:material-code-braces: DatastoreStatisticsTypeDef](./type_defs.md#datastorestatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FileFormatConfigurationTypeDef

```python
# FileFormatConfigurationTypeDef definition

class FileFormatConfigurationTypeDef(TypedDict):
    jsonConfiguration: NotRequired[Mapping[str, Any]],
    parquetConfiguration: NotRequired[ParquetConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ParquetConfigurationTypeDef](./type_defs.md#parquetconfigurationtypedef) [:material-code-braces: ParquetConfigurationOutputTypeDef](./type_defs.md#parquetconfigurationoutputtypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    dataset: DatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatasetRequestRequestTypeDef

```python
# UpdateDatasetRequestRequestTypeDef definition

class UpdateDatasetRequestRequestTypeDef(TypedDict):
    datasetName: str,
    actions: Sequence[DatasetActionTypeDef],  # (1)
    triggers: NotRequired[Sequence[DatasetTriggerTypeDef]],  # (2)
    contentDeliveryRules: NotRequired[Sequence[DatasetContentDeliveryRuleTypeDef]],  # (3)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (4)
    versioningConfiguration: NotRequired[VersioningConfigurationTypeDef],  # (5)
    lateDataRules: NotRequired[Sequence[LateDataRuleTypeDef]],  # (6)
```

1. See [:material-code-braces: DatasetActionTypeDef](./type_defs.md#datasetactiontypedef) 
2. See [:material-code-braces: DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef) 
3. See [:material-code-braces: DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
6. See [:material-code-braces: LateDataRuleTypeDef](./type_defs.md#latedataruletypedef) 
## CreateDatastoreRequestRequestTypeDef

```python
# CreateDatastoreRequestRequestTypeDef definition

class CreateDatastoreRequestRequestTypeDef(TypedDict):
    datastoreName: str,
    datastoreStorage: NotRequired[DatastoreStorageTypeDef],  # (1)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    fileFormatConfiguration: NotRequired[FileFormatConfigurationTypeDef],  # (4)
    datastorePartitions: NotRequired[DatastorePartitionsTypeDef],  # (5)
```

1. See [:material-code-braces: DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef) 
5. See [:material-code-braces: DatastorePartitionsTypeDef](./type_defs.md#datastorepartitionstypedef) 
## UpdateDatastoreRequestRequestTypeDef

```python
# UpdateDatastoreRequestRequestTypeDef definition

class UpdateDatastoreRequestRequestTypeDef(TypedDict):
    datastoreName: str,
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (1)
    datastoreStorage: NotRequired[DatastoreStorageTypeDef],  # (2)
    fileFormatConfiguration: NotRequired[FileFormatConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef) 
3. See [:material-code-braces: FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef) 
## CreateDatasetRequestRequestTypeDef

```python
# CreateDatasetRequestRequestTypeDef definition

class CreateDatasetRequestRequestTypeDef(TypedDict):
    datasetName: str,
    actions: Sequence[DatasetActionUnionTypeDef],  # (1)
    triggers: NotRequired[Sequence[DatasetTriggerTypeDef]],  # (2)
    contentDeliveryRules: NotRequired[Sequence[DatasetContentDeliveryRuleTypeDef]],  # (3)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (4)
    versioningConfiguration: NotRequired[VersioningConfigurationTypeDef],  # (5)
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    lateDataRules: NotRequired[Sequence[LateDataRuleTypeDef]],  # (7)
```

1. See [:material-code-braces: DatasetActionTypeDef](./type_defs.md#datasetactiontypedef) [:material-code-braces: DatasetActionOutputTypeDef](./type_defs.md#datasetactionoutputtypedef) 
2. See [:material-code-braces: DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef) 
3. See [:material-code-braces: DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: LateDataRuleTypeDef](./type_defs.md#latedataruletypedef) 
