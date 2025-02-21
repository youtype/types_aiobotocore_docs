# Type definitions

> [Index](../README.md) > [IoTAnalytics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# TimestampTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AddAttributesActivityUnionTypeDef

```python
# AddAttributesActivityUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityUnionTypeDef


def get_value() -> AddAttributesActivityUnionTypeDef:
    return ...


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
# RemoveAttributesActivityUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import RemoveAttributesActivityUnionTypeDef


def get_value() -> RemoveAttributesActivityUnionTypeDef:
    return ...


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
# SelectAttributesActivityUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import SelectAttributesActivityUnionTypeDef


def get_value() -> SelectAttributesActivityUnionTypeDef:
    return ...


# SelectAttributesActivityUnionTypeDef definition

SelectAttributesActivityUnionTypeDef = Union[
    SelectAttributesActivityTypeDef,  # (1)
    SelectAttributesActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SelectAttributesActivityTypeDef](./type_defs.md#selectattributesactivitytypedef) 
2. See [:material-code-braces: SelectAttributesActivityOutputTypeDef](./type_defs.md#selectattributesactivityoutputtypedef) 

## ChannelStorageUnionTypeDef

```python
# ChannelStorageUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelStorageUnionTypeDef


def get_value() -> ChannelStorageUnionTypeDef:
    return ...


# ChannelStorageUnionTypeDef definition

ChannelStorageUnionTypeDef = Union[
    ChannelStorageTypeDef,  # (1)
    ChannelStorageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef) 
2. See [:material-code-braces: ChannelStorageOutputTypeDef](./type_defs.md#channelstorageoutputtypedef) 

## DatastoreStorageUnionTypeDef

```python
# DatastoreStorageUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreStorageUnionTypeDef


def get_value() -> DatastoreStorageUnionTypeDef:
    return ...


# DatastoreStorageUnionTypeDef definition

DatastoreStorageUnionTypeDef = Union[
    DatastoreStorageTypeDef,  # (1)
    DatastoreStorageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef) 
2. See [:material-code-braces: DatastoreStorageOutputTypeDef](./type_defs.md#datastorestorageoutputtypedef) 

## DatastorePartitionsUnionTypeDef

```python
# DatastorePartitionsUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import DatastorePartitionsUnionTypeDef


def get_value() -> DatastorePartitionsUnionTypeDef:
    return ...


# DatastorePartitionsUnionTypeDef definition

DatastorePartitionsUnionTypeDef = Union[
    DatastorePartitionsTypeDef,  # (1)
    DatastorePartitionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatastorePartitionsTypeDef](./type_defs.md#datastorepartitionstypedef) 
2. See [:material-code-braces: DatastorePartitionsOutputTypeDef](./type_defs.md#datastorepartitionsoutputtypedef) 

## SqlQueryDatasetActionUnionTypeDef

```python
# SqlQueryDatasetActionUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import SqlQueryDatasetActionUnionTypeDef


def get_value() -> SqlQueryDatasetActionUnionTypeDef:
    return ...


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
# ContainerDatasetActionUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import ContainerDatasetActionUnionTypeDef


def get_value() -> ContainerDatasetActionUnionTypeDef:
    return ...


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
# PipelineActivityUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import PipelineActivityUnionTypeDef


def get_value() -> PipelineActivityUnionTypeDef:
    return ...


# PipelineActivityUnionTypeDef definition

PipelineActivityUnionTypeDef = Union[
    PipelineActivityTypeDef,  # (1)
    PipelineActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) 
2. See [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 

## FileFormatConfigurationUnionTypeDef

```python
# FileFormatConfigurationUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import FileFormatConfigurationUnionTypeDef


def get_value() -> FileFormatConfigurationUnionTypeDef:
    return ...


# FileFormatConfigurationUnionTypeDef definition

FileFormatConfigurationUnionTypeDef = Union[
    FileFormatConfigurationTypeDef,  # (1)
    FileFormatConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef) 
2. See [:material-code-braces: FileFormatConfigurationOutputTypeDef](./type_defs.md#fileformatconfigurationoutputtypedef) 

## DatasetActionUnionTypeDef

```python
# DatasetActionUnionTypeDef Union usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetActionUnionTypeDef


def get_value() -> DatasetActionUnionTypeDef:
    return ...


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
# AddAttributesActivityOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef


def get_value() -> AddAttributesActivityOutputTypeDef:
    return {
        "name": ...,
    }


# AddAttributesActivityOutputTypeDef definition

class AddAttributesActivityOutputTypeDef(TypedDict):
    name: str,
    attributes: Dict[str, str],
    next: NotRequired[str],
```

## AddAttributesActivityTypeDef

```python
# AddAttributesActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityTypeDef


def get_value() -> AddAttributesActivityTypeDef:
    return {
        "name": ...,
    }


# AddAttributesActivityTypeDef definition

class AddAttributesActivityTypeDef(TypedDict):
    name: str,
    attributes: Mapping[str, str],
    next: NotRequired[str],
```

## BatchPutMessageErrorEntryTypeDef

```python
# BatchPutMessageErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageErrorEntryTypeDef


def get_value() -> BatchPutMessageErrorEntryTypeDef:
    return {
        "messageId": ...,
    }


# BatchPutMessageErrorEntryTypeDef definition

class BatchPutMessageErrorEntryTypeDef(TypedDict):
    messageId: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ResponseMetadataTypeDef


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

## CancelPipelineReprocessingRequestTypeDef

```python
# CancelPipelineReprocessingRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CancelPipelineReprocessingRequestTypeDef


def get_value() -> CancelPipelineReprocessingRequestTypeDef:
    return {
        "pipelineName": ...,
    }


# CancelPipelineReprocessingRequestTypeDef definition

class CancelPipelineReprocessingRequestTypeDef(TypedDict):
    pipelineName: str,
    reprocessingId: str,
```

## ChannelActivityTypeDef

```python
# ChannelActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelActivityTypeDef


def get_value() -> ChannelActivityTypeDef:
    return {
        "name": ...,
    }


# ChannelActivityTypeDef definition

class ChannelActivityTypeDef(TypedDict):
    name: str,
    channelName: str,
    next: NotRequired[str],
```

## ChannelMessagesTypeDef

```python
# ChannelMessagesTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelMessagesTypeDef


def get_value() -> ChannelMessagesTypeDef:
    return {
        "s3Paths": ...,
    }


# ChannelMessagesTypeDef definition

class ChannelMessagesTypeDef(TypedDict):
    s3Paths: NotRequired[Sequence[str]],
```

## EstimatedResourceSizeTypeDef

```python
# EstimatedResourceSizeTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import EstimatedResourceSizeTypeDef


def get_value() -> EstimatedResourceSizeTypeDef:
    return {
        "estimatedSizeInBytes": ...,
    }


# EstimatedResourceSizeTypeDef definition

class EstimatedResourceSizeTypeDef(TypedDict):
    estimatedSizeInBytes: NotRequired[float],
    estimatedOn: NotRequired[datetime],
```

## CustomerManagedChannelS3StorageTypeDef

```python
# CustomerManagedChannelS3StorageTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CustomerManagedChannelS3StorageTypeDef


def get_value() -> CustomerManagedChannelS3StorageTypeDef:
    return {
        "bucket": ...,
    }


# CustomerManagedChannelS3StorageTypeDef definition

class CustomerManagedChannelS3StorageTypeDef(TypedDict):
    bucket: str,
    roleArn: str,
    keyPrefix: NotRequired[str],
```

## CustomerManagedChannelS3StorageSummaryTypeDef

```python
# CustomerManagedChannelS3StorageSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CustomerManagedChannelS3StorageSummaryTypeDef


def get_value() -> CustomerManagedChannelS3StorageSummaryTypeDef:
    return {
        "bucket": ...,
    }


# CustomerManagedChannelS3StorageSummaryTypeDef definition

class CustomerManagedChannelS3StorageSummaryTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
    roleArn: NotRequired[str],
```

## RetentionPeriodTypeDef

```python
# RetentionPeriodTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import RetentionPeriodTypeDef


def get_value() -> RetentionPeriodTypeDef:
    return {
        "unlimited": ...,
    }


# RetentionPeriodTypeDef definition

class RetentionPeriodTypeDef(TypedDict):
    unlimited: NotRequired[bool],
    numberOfDays: NotRequired[int],
```

## ColumnTypeDef

```python
# ColumnTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ColumnTypeDef


def get_value() -> ColumnTypeDef:
    return {
        "name": ...,
    }


# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    name: str,
    type: str,
```

## ResourceConfigurationTypeDef

```python
# ResourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ResourceConfigurationTypeDef


def get_value() -> ResourceConfigurationTypeDef:
    return {
        "computeType": ...,
    }


# ResourceConfigurationTypeDef definition

class ResourceConfigurationTypeDef(TypedDict):
    computeType: ComputeTypeType,  # (1)
    volumeSizeInGB: int,
```

1. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## CreateDatasetContentRequestTypeDef

```python
# CreateDatasetContentRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateDatasetContentRequestTypeDef


def get_value() -> CreateDatasetContentRequestTypeDef:
    return {
        "datasetName": ...,
    }


# CreateDatasetContentRequestTypeDef definition

class CreateDatasetContentRequestTypeDef(TypedDict):
    datasetName: str,
    versionId: NotRequired[str],
```

## VersioningConfigurationTypeDef

```python
# VersioningConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import VersioningConfigurationTypeDef


def get_value() -> VersioningConfigurationTypeDef:
    return {
        "unlimited": ...,
    }


# VersioningConfigurationTypeDef definition

class VersioningConfigurationTypeDef(TypedDict):
    unlimited: NotRequired[bool],
    maxVersions: NotRequired[int],
```

## CustomerManagedDatastoreS3StorageSummaryTypeDef

```python
# CustomerManagedDatastoreS3StorageSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CustomerManagedDatastoreS3StorageSummaryTypeDef


def get_value() -> CustomerManagedDatastoreS3StorageSummaryTypeDef:
    return {
        "bucket": ...,
    }


# CustomerManagedDatastoreS3StorageSummaryTypeDef definition

class CustomerManagedDatastoreS3StorageSummaryTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
    roleArn: NotRequired[str],
```

## CustomerManagedDatastoreS3StorageTypeDef

```python
# CustomerManagedDatastoreS3StorageTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CustomerManagedDatastoreS3StorageTypeDef


def get_value() -> CustomerManagedDatastoreS3StorageTypeDef:
    return {
        "bucket": ...,
    }


# CustomerManagedDatastoreS3StorageTypeDef definition

class CustomerManagedDatastoreS3StorageTypeDef(TypedDict):
    bucket: str,
    roleArn: str,
    keyPrefix: NotRequired[str],
```

## DatasetActionSummaryTypeDef

```python
# DatasetActionSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetActionSummaryTypeDef


def get_value() -> DatasetActionSummaryTypeDef:
    return {
        "actionName": ...,
    }


# DatasetActionSummaryTypeDef definition

class DatasetActionSummaryTypeDef(TypedDict):
    actionName: NotRequired[str],
    actionType: NotRequired[DatasetActionTypeType],  # (1)
```

1. See [:material-code-brackets: DatasetActionTypeType](./literals.md#datasetactiontypetype) 
## IotEventsDestinationConfigurationTypeDef

```python
# IotEventsDestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import IotEventsDestinationConfigurationTypeDef


def get_value() -> IotEventsDestinationConfigurationTypeDef:
    return {
        "inputName": ...,
    }


# IotEventsDestinationConfigurationTypeDef definition

class IotEventsDestinationConfigurationTypeDef(TypedDict):
    inputName: str,
    roleArn: str,
```

## DatasetContentStatusTypeDef

```python
# DatasetContentStatusTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetContentStatusTypeDef


def get_value() -> DatasetContentStatusTypeDef:
    return {
        "state": ...,
    }


# DatasetContentStatusTypeDef definition

class DatasetContentStatusTypeDef(TypedDict):
    state: NotRequired[DatasetContentStateType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: DatasetContentStateType](./literals.md#datasetcontentstatetype) 
## DatasetContentVersionValueTypeDef

```python
# DatasetContentVersionValueTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetContentVersionValueTypeDef


def get_value() -> DatasetContentVersionValueTypeDef:
    return {
        "datasetName": ...,
    }


# DatasetContentVersionValueTypeDef definition

class DatasetContentVersionValueTypeDef(TypedDict):
    datasetName: str,
```

## DatasetEntryTypeDef

```python
# DatasetEntryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetEntryTypeDef


def get_value() -> DatasetEntryTypeDef:
    return {
        "entryName": ...,
    }


# DatasetEntryTypeDef definition

class DatasetEntryTypeDef(TypedDict):
    entryName: NotRequired[str],
    dataURI: NotRequired[str],
```

## ScheduleTypeDef

```python
# ScheduleTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ScheduleTypeDef


def get_value() -> ScheduleTypeDef:
    return {
        "expression": ...,
    }


# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    expression: NotRequired[str],
```

## TriggeringDatasetTypeDef

```python
# TriggeringDatasetTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import TriggeringDatasetTypeDef


def get_value() -> TriggeringDatasetTypeDef:
    return {
        "name": ...,
    }


# TriggeringDatasetTypeDef definition

class TriggeringDatasetTypeDef(TypedDict):
    name: str,
```

## DatastoreActivityTypeDef

```python
# DatastoreActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreActivityTypeDef


def get_value() -> DatastoreActivityTypeDef:
    return {
        "name": ...,
    }


# DatastoreActivityTypeDef definition

class DatastoreActivityTypeDef(TypedDict):
    name: str,
    datastoreName: str,
```

## IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef

```python
# IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef


def get_value() -> IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef:
    return {
        "bucket": ...,
    }


# IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef definition

class IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
```

## IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef

```python
# IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef


def get_value() -> IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef:
    return {
        "bucket": ...,
    }


# IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef definition

class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(TypedDict):
    bucket: str,
    keyPrefix: NotRequired[str],
```

## PartitionTypeDef

```python
# PartitionTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import PartitionTypeDef


def get_value() -> PartitionTypeDef:
    return {
        "attributeName": ...,
    }


# PartitionTypeDef definition

class PartitionTypeDef(TypedDict):
    attributeName: str,
```

## TimestampPartitionTypeDef

```python
# TimestampPartitionTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import TimestampPartitionTypeDef


def get_value() -> TimestampPartitionTypeDef:
    return {
        "attributeName": ...,
    }


# TimestampPartitionTypeDef definition

class TimestampPartitionTypeDef(TypedDict):
    attributeName: str,
    timestampFormat: NotRequired[str],
```

## DeleteChannelRequestTypeDef

```python
# DeleteChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeleteChannelRequestTypeDef


def get_value() -> DeleteChannelRequestTypeDef:
    return {
        "channelName": ...,
    }


# DeleteChannelRequestTypeDef definition

class DeleteChannelRequestTypeDef(TypedDict):
    channelName: str,
```

## DeleteDatasetContentRequestTypeDef

```python
# DeleteDatasetContentRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeleteDatasetContentRequestTypeDef


def get_value() -> DeleteDatasetContentRequestTypeDef:
    return {
        "datasetName": ...,
    }


# DeleteDatasetContentRequestTypeDef definition

class DeleteDatasetContentRequestTypeDef(TypedDict):
    datasetName: str,
    versionId: NotRequired[str],
```

## DeleteDatasetRequestTypeDef

```python
# DeleteDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeleteDatasetRequestTypeDef


def get_value() -> DeleteDatasetRequestTypeDef:
    return {
        "datasetName": ...,
    }


# DeleteDatasetRequestTypeDef definition

class DeleteDatasetRequestTypeDef(TypedDict):
    datasetName: str,
```

## DeleteDatastoreRequestTypeDef

```python
# DeleteDatastoreRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeleteDatastoreRequestTypeDef


def get_value() -> DeleteDatastoreRequestTypeDef:
    return {
        "datastoreName": ...,
    }


# DeleteDatastoreRequestTypeDef definition

class DeleteDatastoreRequestTypeDef(TypedDict):
    datastoreName: str,
```

## DeletePipelineRequestTypeDef

```python
# DeletePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeletePipelineRequestTypeDef


def get_value() -> DeletePipelineRequestTypeDef:
    return {
        "pipelineName": ...,
    }


# DeletePipelineRequestTypeDef definition

class DeletePipelineRequestTypeDef(TypedDict):
    pipelineName: str,
```

## DeltaTimeSessionWindowConfigurationTypeDef

```python
# DeltaTimeSessionWindowConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeltaTimeSessionWindowConfigurationTypeDef


def get_value() -> DeltaTimeSessionWindowConfigurationTypeDef:
    return {
        "timeoutInMinutes": ...,
    }


# DeltaTimeSessionWindowConfigurationTypeDef definition

class DeltaTimeSessionWindowConfigurationTypeDef(TypedDict):
    timeoutInMinutes: int,
```

## DeltaTimeTypeDef

```python
# DeltaTimeTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeltaTimeTypeDef


def get_value() -> DeltaTimeTypeDef:
    return {
        "offsetSeconds": ...,
    }


# DeltaTimeTypeDef definition

class DeltaTimeTypeDef(TypedDict):
    offsetSeconds: int,
    timeExpression: str,
```

## DescribeChannelRequestTypeDef

```python
# DescribeChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribeChannelRequestTypeDef


def get_value() -> DescribeChannelRequestTypeDef:
    return {
        "channelName": ...,
    }


# DescribeChannelRequestTypeDef definition

class DescribeChannelRequestTypeDef(TypedDict):
    channelName: str,
    includeStatistics: NotRequired[bool],
```

## DescribeDatasetRequestTypeDef

```python
# DescribeDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribeDatasetRequestTypeDef


def get_value() -> DescribeDatasetRequestTypeDef:
    return {
        "datasetName": ...,
    }


# DescribeDatasetRequestTypeDef definition

class DescribeDatasetRequestTypeDef(TypedDict):
    datasetName: str,
```

## DescribeDatastoreRequestTypeDef

```python
# DescribeDatastoreRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribeDatastoreRequestTypeDef


def get_value() -> DescribeDatastoreRequestTypeDef:
    return {
        "datastoreName": ...,
    }


# DescribeDatastoreRequestTypeDef definition

class DescribeDatastoreRequestTypeDef(TypedDict):
    datastoreName: str,
    includeStatistics: NotRequired[bool],
```

## LoggingOptionsTypeDef

```python
# LoggingOptionsTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import LoggingOptionsTypeDef


def get_value() -> LoggingOptionsTypeDef:
    return {
        "roleArn": ...,
    }


# LoggingOptionsTypeDef definition

class LoggingOptionsTypeDef(TypedDict):
    roleArn: str,
    level: LoggingLevelType,  # (1)
    enabled: bool,
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## DescribePipelineRequestTypeDef

```python
# DescribePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribePipelineRequestTypeDef


def get_value() -> DescribePipelineRequestTypeDef:
    return {
        "pipelineName": ...,
    }


# DescribePipelineRequestTypeDef definition

class DescribePipelineRequestTypeDef(TypedDict):
    pipelineName: str,
```

## DeviceRegistryEnrichActivityTypeDef

```python
# DeviceRegistryEnrichActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeviceRegistryEnrichActivityTypeDef


def get_value() -> DeviceRegistryEnrichActivityTypeDef:
    return {
        "name": ...,
    }


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
# DeviceShadowEnrichActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DeviceShadowEnrichActivityTypeDef


def get_value() -> DeviceShadowEnrichActivityTypeDef:
    return {
        "name": ...,
    }


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
# FilterActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import FilterActivityTypeDef


def get_value() -> FilterActivityTypeDef:
    return {
        "name": ...,
    }


# FilterActivityTypeDef definition

class FilterActivityTypeDef(TypedDict):
    name: str,
    filter: str,
    next: NotRequired[str],
```

## GetDatasetContentRequestTypeDef

```python
# GetDatasetContentRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import GetDatasetContentRequestTypeDef


def get_value() -> GetDatasetContentRequestTypeDef:
    return {
        "datasetName": ...,
    }


# GetDatasetContentRequestTypeDef definition

class GetDatasetContentRequestTypeDef(TypedDict):
    datasetName: str,
    versionId: NotRequired[str],
```

## GlueConfigurationTypeDef

```python
# GlueConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import GlueConfigurationTypeDef


def get_value() -> GlueConfigurationTypeDef:
    return {
        "tableName": ...,
    }


# GlueConfigurationTypeDef definition

class GlueConfigurationTypeDef(TypedDict):
    tableName: str,
    databaseName: str,
```

## LambdaActivityTypeDef

```python
# LambdaActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import LambdaActivityTypeDef


def get_value() -> LambdaActivityTypeDef:
    return {
        "name": ...,
    }


# LambdaActivityTypeDef definition

class LambdaActivityTypeDef(TypedDict):
    name: str,
    lambdaName: str,
    batchSize: int,
    next: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChannelsRequestTypeDef

```python
# ListChannelsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListChannelsRequestTypeDef


def get_value() -> ListChannelsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListChannelsRequestTypeDef definition

class ListChannelsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDatasetsRequestTypeDef

```python
# ListDatasetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatasetsRequestTypeDef


def get_value() -> ListDatasetsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListDatasetsRequestTypeDef definition

class ListDatasetsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDatastoresRequestTypeDef

```python
# ListDatastoresRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatastoresRequestTypeDef


def get_value() -> ListDatastoresRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListDatastoresRequestTypeDef definition

class ListDatastoresRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPipelinesRequestTypeDef

```python
# ListPipelinesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListPipelinesRequestTypeDef


def get_value() -> ListPipelinesRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListPipelinesRequestTypeDef definition

class ListPipelinesRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MathActivityTypeDef

```python
# MathActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import MathActivityTypeDef


def get_value() -> MathActivityTypeDef:
    return {
        "name": ...,
    }


# MathActivityTypeDef definition

class MathActivityTypeDef(TypedDict):
    name: str,
    attribute: str,
    math: str,
    next: NotRequired[str],
```

## OutputFileUriValueTypeDef

```python
# OutputFileUriValueTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import OutputFileUriValueTypeDef


def get_value() -> OutputFileUriValueTypeDef:
    return {
        "fileName": ...,
    }


# OutputFileUriValueTypeDef definition

class OutputFileUriValueTypeDef(TypedDict):
    fileName: str,
```

## RemoveAttributesActivityOutputTypeDef

```python
# RemoveAttributesActivityOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import RemoveAttributesActivityOutputTypeDef


def get_value() -> RemoveAttributesActivityOutputTypeDef:
    return {
        "name": ...,
    }


# RemoveAttributesActivityOutputTypeDef definition

class RemoveAttributesActivityOutputTypeDef(TypedDict):
    name: str,
    attributes: List[str],
    next: NotRequired[str],
```

## SelectAttributesActivityOutputTypeDef

```python
# SelectAttributesActivityOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SelectAttributesActivityOutputTypeDef


def get_value() -> SelectAttributesActivityOutputTypeDef:
    return {
        "name": ...,
    }


# SelectAttributesActivityOutputTypeDef definition

class SelectAttributesActivityOutputTypeDef(TypedDict):
    name: str,
    attributes: List[str],
    next: NotRequired[str],
```

## ReprocessingSummaryTypeDef

```python
# ReprocessingSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ReprocessingSummaryTypeDef


def get_value() -> ReprocessingSummaryTypeDef:
    return {
        "id": ...,
    }


# ReprocessingSummaryTypeDef definition

class ReprocessingSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    status: NotRequired[ReprocessingStatusType],  # (1)
    creationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReprocessingStatusType](./literals.md#reprocessingstatustype) 
## RemoveAttributesActivityTypeDef

```python
# RemoveAttributesActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import RemoveAttributesActivityTypeDef


def get_value() -> RemoveAttributesActivityTypeDef:
    return {
        "name": ...,
    }


# RemoveAttributesActivityTypeDef definition

class RemoveAttributesActivityTypeDef(TypedDict):
    name: str,
    attributes: Sequence[str],
    next: NotRequired[str],
```

## SelectAttributesActivityTypeDef

```python
# SelectAttributesActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SelectAttributesActivityTypeDef


def get_value() -> SelectAttributesActivityTypeDef:
    return {
        "name": ...,
    }


# SelectAttributesActivityTypeDef definition

class SelectAttributesActivityTypeDef(TypedDict):
    name: str,
    attributes: Sequence[str],
    next: NotRequired[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## BatchPutMessageResponseTypeDef

```python
# BatchPutMessageResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageResponseTypeDef


def get_value() -> BatchPutMessageResponseTypeDef:
    return {
        "batchPutMessageErrorEntries": ...,
    }


# BatchPutMessageResponseTypeDef definition

class BatchPutMessageResponseTypeDef(TypedDict):
    batchPutMessageErrorEntries: List[BatchPutMessageErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutMessageErrorEntryTypeDef](./type_defs.md#batchputmessageerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetContentResponseTypeDef

```python
# CreateDatasetContentResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateDatasetContentResponseTypeDef


def get_value() -> CreateDatasetContentResponseTypeDef:
    return {
        "versionId": ...,
    }


# CreateDatasetContentResponseTypeDef definition

class CreateDatasetContentResponseTypeDef(TypedDict):
    versionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineResponseTypeDef

```python
# CreatePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreatePipelineResponseTypeDef


def get_value() -> CreatePipelineResponseTypeDef:
    return {
        "pipelineName": ...,
    }


# CreatePipelineResponseTypeDef definition

class CreatePipelineResponseTypeDef(TypedDict):
    pipelineName: str,
    pipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunPipelineActivityResponseTypeDef

```python
# RunPipelineActivityResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import RunPipelineActivityResponseTypeDef


def get_value() -> RunPipelineActivityResponseTypeDef:
    return {
        "payloads": ...,
    }


# RunPipelineActivityResponseTypeDef definition

class RunPipelineActivityResponseTypeDef(TypedDict):
    payloads: List[bytes],
    logResult: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SampleChannelDataResponseTypeDef

```python
# SampleChannelDataResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SampleChannelDataResponseTypeDef


def get_value() -> SampleChannelDataResponseTypeDef:
    return {
        "payloads": ...,
    }


# SampleChannelDataResponseTypeDef definition

class SampleChannelDataResponseTypeDef(TypedDict):
    payloads: List[bytes],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPipelineReprocessingResponseTypeDef

```python
# StartPipelineReprocessingResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import StartPipelineReprocessingResponseTypeDef


def get_value() -> StartPipelineReprocessingResponseTypeDef:
    return {
        "reprocessingId": ...,
    }


# StartPipelineReprocessingResponseTypeDef definition

class StartPipelineReprocessingResponseTypeDef(TypedDict):
    reprocessingId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageTypeDef

```python
# MessageTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import MessageTypeDef


def get_value() -> MessageTypeDef:
    return {
        "messageId": ...,
    }


# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    messageId: str,
    payload: BlobTypeDef,
```

## ChannelStatisticsTypeDef

```python
# ChannelStatisticsTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelStatisticsTypeDef


def get_value() -> ChannelStatisticsTypeDef:
    return {
        "size": ...,
    }


# ChannelStatisticsTypeDef definition

class ChannelStatisticsTypeDef(TypedDict):
    size: NotRequired[EstimatedResourceSizeTypeDef],  # (1)
```

1. See [:material-code-braces: EstimatedResourceSizeTypeDef](./type_defs.md#estimatedresourcesizetypedef) 
## DatastoreStatisticsTypeDef

```python
# DatastoreStatisticsTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreStatisticsTypeDef


def get_value() -> DatastoreStatisticsTypeDef:
    return {
        "size": ...,
    }


# DatastoreStatisticsTypeDef definition

class DatastoreStatisticsTypeDef(TypedDict):
    size: NotRequired[EstimatedResourceSizeTypeDef],  # (1)
```

1. See [:material-code-braces: EstimatedResourceSizeTypeDef](./type_defs.md#estimatedresourcesizetypedef) 
## ChannelStorageOutputTypeDef

```python
# ChannelStorageOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelStorageOutputTypeDef


def get_value() -> ChannelStorageOutputTypeDef:
    return {
        "serviceManagedS3": ...,
    }


# ChannelStorageOutputTypeDef definition

class ChannelStorageOutputTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Dict[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedChannelS3StorageTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerManagedChannelS3StorageTypeDef](./type_defs.md#customermanagedchannels3storagetypedef) 
## ChannelStorageTypeDef

```python
# ChannelStorageTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelStorageTypeDef


def get_value() -> ChannelStorageTypeDef:
    return {
        "serviceManagedS3": ...,
    }


# ChannelStorageTypeDef definition

class ChannelStorageTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Mapping[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedChannelS3StorageTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerManagedChannelS3StorageTypeDef](./type_defs.md#customermanagedchannels3storagetypedef) 
## ChannelStorageSummaryTypeDef

```python
# ChannelStorageSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelStorageSummaryTypeDef


def get_value() -> ChannelStorageSummaryTypeDef:
    return {
        "serviceManagedS3": ...,
    }


# ChannelStorageSummaryTypeDef definition

class ChannelStorageSummaryTypeDef(TypedDict):
    serviceManagedS3: NotRequired[Dict[str, Any]],
    customerManagedS3: NotRequired[CustomerManagedChannelS3StorageSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerManagedChannelS3StorageSummaryTypeDef](./type_defs.md#customermanagedchannels3storagesummarytypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateChannelResponseTypeDef


def get_value() -> CreateChannelResponseTypeDef:
    return {
        "channelName": ...,
    }


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
# CreateDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateDatasetResponseTypeDef


def get_value() -> CreateDatasetResponseTypeDef:
    return {
        "datasetName": ...,
    }


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
# CreateDatastoreResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateDatastoreResponseTypeDef


def get_value() -> CreateDatastoreResponseTypeDef:
    return {
        "datastoreName": ...,
    }


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
# SchemaDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SchemaDefinitionOutputTypeDef


def get_value() -> SchemaDefinitionOutputTypeDef:
    return {
        "columns": ...,
    }


# SchemaDefinitionOutputTypeDef definition

class SchemaDefinitionOutputTypeDef(TypedDict):
    columns: NotRequired[List[ColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
## SchemaDefinitionTypeDef

```python
# SchemaDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SchemaDefinitionTypeDef


def get_value() -> SchemaDefinitionTypeDef:
    return {
        "columns": ...,
    }


# SchemaDefinitionTypeDef definition

class SchemaDefinitionTypeDef(TypedDict):
    columns: NotRequired[Sequence[ColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DatasetContentSummaryTypeDef

```python
# DatasetContentSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetContentSummaryTypeDef


def get_value() -> DatasetContentSummaryTypeDef:
    return {
        "version": ...,
    }


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
# GetDatasetContentResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import GetDatasetContentResponseTypeDef


def get_value() -> GetDatasetContentResponseTypeDef:
    return {
        "entries": ...,
    }


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
# DatasetTriggerTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetTriggerTypeDef


def get_value() -> DatasetTriggerTypeDef:
    return {
        "schedule": ...,
    }


# DatasetTriggerTypeDef definition

class DatasetTriggerTypeDef(TypedDict):
    schedule: NotRequired[ScheduleTypeDef],  # (1)
    dataset: NotRequired[TriggeringDatasetTypeDef],  # (2)
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: TriggeringDatasetTypeDef](./type_defs.md#triggeringdatasettypedef) 
## DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef

```python
# DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef


def get_value() -> DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef:
    return {
        "customerManagedS3Storage": ...,
    }


# DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef definition

class DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef(TypedDict):
    customerManagedS3Storage: NotRequired[IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagesummarytypedef) 
## DatastoreIotSiteWiseMultiLayerStorageTypeDef

```python
# DatastoreIotSiteWiseMultiLayerStorageTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreIotSiteWiseMultiLayerStorageTypeDef


def get_value() -> DatastoreIotSiteWiseMultiLayerStorageTypeDef:
    return {
        "customerManagedS3Storage": ...,
    }


# DatastoreIotSiteWiseMultiLayerStorageTypeDef definition

class DatastoreIotSiteWiseMultiLayerStorageTypeDef(TypedDict):
    customerManagedS3Storage: IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,  # (1)
```

1. See [:material-code-braces: IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagetypedef) 
## DatastorePartitionTypeDef

```python
# DatastorePartitionTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastorePartitionTypeDef


def get_value() -> DatastorePartitionTypeDef:
    return {
        "attributePartition": ...,
    }


# DatastorePartitionTypeDef definition

class DatastorePartitionTypeDef(TypedDict):
    attributePartition: NotRequired[PartitionTypeDef],  # (1)
    timestampPartition: NotRequired[TimestampPartitionTypeDef],  # (2)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: TimestampPartitionTypeDef](./type_defs.md#timestamppartitiontypedef) 
## LateDataRuleConfigurationTypeDef

```python
# LateDataRuleConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import LateDataRuleConfigurationTypeDef


def get_value() -> LateDataRuleConfigurationTypeDef:
    return {
        "deltaTimeSessionWindowConfiguration": ...,
    }


# LateDataRuleConfigurationTypeDef definition

class LateDataRuleConfigurationTypeDef(TypedDict):
    deltaTimeSessionWindowConfiguration: NotRequired[DeltaTimeSessionWindowConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DeltaTimeSessionWindowConfigurationTypeDef](./type_defs.md#deltatimesessionwindowconfigurationtypedef) 
## QueryFilterTypeDef

```python
# QueryFilterTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import QueryFilterTypeDef


def get_value() -> QueryFilterTypeDef:
    return {
        "deltaTime": ...,
    }


# QueryFilterTypeDef definition

class QueryFilterTypeDef(TypedDict):
    deltaTime: NotRequired[DeltaTimeTypeDef],  # (1)
```

1. See [:material-code-braces: DeltaTimeTypeDef](./type_defs.md#deltatimetypedef) 
## DescribeLoggingOptionsResponseTypeDef

```python
# DescribeLoggingOptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribeLoggingOptionsResponseTypeDef


def get_value() -> DescribeLoggingOptionsResponseTypeDef:
    return {
        "loggingOptions": ...,
    }


# DescribeLoggingOptionsResponseTypeDef definition

class DescribeLoggingOptionsResponseTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingOptionsRequestTypeDef

```python
# PutLoggingOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import PutLoggingOptionsRequestTypeDef


def get_value() -> PutLoggingOptionsRequestTypeDef:
    return {
        "loggingOptions": ...,
    }


# PutLoggingOptionsRequestTypeDef definition

class PutLoggingOptionsRequestTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import S3DestinationConfigurationTypeDef


def get_value() -> S3DestinationConfigurationTypeDef:
    return {
        "bucket": ...,
    }


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
# ListChannelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListChannelsRequestPaginateTypeDef


def get_value() -> ListChannelsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListChannelsRequestPaginateTypeDef definition

class ListChannelsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetsRequestPaginateTypeDef

```python
# ListDatasetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatasetsRequestPaginateTypeDef


def get_value() -> ListDatasetsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDatasetsRequestPaginateTypeDef definition

class ListDatasetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatastoresRequestPaginateTypeDef

```python
# ListDatastoresRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatastoresRequestPaginateTypeDef


def get_value() -> ListDatastoresRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDatastoresRequestPaginateTypeDef definition

class ListDatastoresRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelinesRequestPaginateTypeDef

```python
# ListPipelinesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListPipelinesRequestPaginateTypeDef


def get_value() -> ListPipelinesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListPipelinesRequestPaginateTypeDef definition

class ListPipelinesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetContentsRequestPaginateTypeDef

```python
# ListDatasetContentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatasetContentsRequestPaginateTypeDef


def get_value() -> ListDatasetContentsRequestPaginateTypeDef:
    return {
        "datasetName": ...,
    }


# ListDatasetContentsRequestPaginateTypeDef definition

class ListDatasetContentsRequestPaginateTypeDef(TypedDict):
    datasetName: str,
    scheduledOnOrAfter: NotRequired[TimestampTypeDef],
    scheduledBefore: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetContentsRequestTypeDef

```python
# ListDatasetContentsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatasetContentsRequestTypeDef


def get_value() -> ListDatasetContentsRequestTypeDef:
    return {
        "datasetName": ...,
    }


# ListDatasetContentsRequestTypeDef definition

class ListDatasetContentsRequestTypeDef(TypedDict):
    datasetName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    scheduledOnOrAfter: NotRequired[TimestampTypeDef],
    scheduledBefore: NotRequired[TimestampTypeDef],
```

## SampleChannelDataRequestTypeDef

```python
# SampleChannelDataRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SampleChannelDataRequestTypeDef


def get_value() -> SampleChannelDataRequestTypeDef:
    return {
        "channelName": ...,
    }


# SampleChannelDataRequestTypeDef definition

class SampleChannelDataRequestTypeDef(TypedDict):
    channelName: str,
    maxMessages: NotRequired[int],
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
```

## StartPipelineReprocessingRequestTypeDef

```python
# StartPipelineReprocessingRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import StartPipelineReprocessingRequestTypeDef


def get_value() -> StartPipelineReprocessingRequestTypeDef:
    return {
        "pipelineName": ...,
    }


# StartPipelineReprocessingRequestTypeDef definition

class StartPipelineReprocessingRequestTypeDef(TypedDict):
    pipelineName: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    channelMessages: NotRequired[ChannelMessagesTypeDef],  # (1)
```

1. See [:material-code-braces: ChannelMessagesTypeDef](./type_defs.md#channelmessagestypedef) 
## VariableTypeDef

```python
# VariableTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import VariableTypeDef


def get_value() -> VariableTypeDef:
    return {
        "name": ...,
    }


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
# PipelineActivityOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import PipelineActivityOutputTypeDef


def get_value() -> PipelineActivityOutputTypeDef:
    return {
        "channel": ...,
    }


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
# PipelineSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import PipelineSummaryTypeDef


def get_value() -> PipelineSummaryTypeDef:
    return {
        "pipelineName": ...,
    }


# PipelineSummaryTypeDef definition

class PipelineSummaryTypeDef(TypedDict):
    pipelineName: NotRequired[str],
    reprocessingSummaries: NotRequired[List[ReprocessingSummaryTypeDef]],  # (1)
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-braces: ReprocessingSummaryTypeDef](./type_defs.md#reprocessingsummarytypedef) 
## BatchPutMessageRequestTypeDef

```python
# BatchPutMessageRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageRequestTypeDef


def get_value() -> BatchPutMessageRequestTypeDef:
    return {
        "channelName": ...,
    }


# BatchPutMessageRequestTypeDef definition

class BatchPutMessageRequestTypeDef(TypedDict):
    channelName: str,
    messages: Sequence[MessageTypeDef],  # (1)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelTypeDef


def get_value() -> ChannelTypeDef:
    return {
        "name": ...,
    }


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
## ChannelSummaryTypeDef

```python
# ChannelSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ChannelSummaryTypeDef


def get_value() -> ChannelSummaryTypeDef:
    return {
        "channelName": ...,
    }


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
# ParquetConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ParquetConfigurationOutputTypeDef


def get_value() -> ParquetConfigurationOutputTypeDef:
    return {
        "schemaDefinition": ...,
    }


# ParquetConfigurationOutputTypeDef definition

class ParquetConfigurationOutputTypeDef(TypedDict):
    schemaDefinition: NotRequired[SchemaDefinitionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
## ParquetConfigurationTypeDef

```python
# ParquetConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ParquetConfigurationTypeDef


def get_value() -> ParquetConfigurationTypeDef:
    return {
        "schemaDefinition": ...,
    }


# ParquetConfigurationTypeDef definition

class ParquetConfigurationTypeDef(TypedDict):
    schemaDefinition: NotRequired[SchemaDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
## ListDatasetContentsResponseTypeDef

```python
# ListDatasetContentsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatasetContentsResponseTypeDef


def get_value() -> ListDatasetContentsResponseTypeDef:
    return {
        "datasetContentSummaries": ...,
    }


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
# DatasetSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetSummaryTypeDef


def get_value() -> DatasetSummaryTypeDef:
    return {
        "datasetName": ...,
    }


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
# DatastoreStorageSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreStorageSummaryTypeDef


def get_value() -> DatastoreStorageSummaryTypeDef:
    return {
        "serviceManagedS3": ...,
    }


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
# DatastoreStorageOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreStorageOutputTypeDef


def get_value() -> DatastoreStorageOutputTypeDef:
    return {
        "serviceManagedS3": ...,
    }


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
# DatastoreStorageTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreStorageTypeDef


def get_value() -> DatastoreStorageTypeDef:
    return {
        "serviceManagedS3": ...,
    }


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
# DatastorePartitionsOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastorePartitionsOutputTypeDef


def get_value() -> DatastorePartitionsOutputTypeDef:
    return {
        "partitions": ...,
    }


# DatastorePartitionsOutputTypeDef definition

class DatastorePartitionsOutputTypeDef(TypedDict):
    partitions: NotRequired[List[DatastorePartitionTypeDef]],  # (1)
```

1. See [:material-code-braces: DatastorePartitionTypeDef](./type_defs.md#datastorepartitiontypedef) 
## DatastorePartitionsTypeDef

```python
# DatastorePartitionsTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastorePartitionsTypeDef


def get_value() -> DatastorePartitionsTypeDef:
    return {
        "partitions": ...,
    }


# DatastorePartitionsTypeDef definition

class DatastorePartitionsTypeDef(TypedDict):
    partitions: NotRequired[Sequence[DatastorePartitionTypeDef]],  # (1)
```

1. See [:material-code-braces: DatastorePartitionTypeDef](./type_defs.md#datastorepartitiontypedef) 
## LateDataRuleTypeDef

```python
# LateDataRuleTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import LateDataRuleTypeDef


def get_value() -> LateDataRuleTypeDef:
    return {
        "ruleName": ...,
    }


# LateDataRuleTypeDef definition

class LateDataRuleTypeDef(TypedDict):
    ruleConfiguration: LateDataRuleConfigurationTypeDef,  # (1)
    ruleName: NotRequired[str],
```

1. See [:material-code-braces: LateDataRuleConfigurationTypeDef](./type_defs.md#latedataruleconfigurationtypedef) 
## SqlQueryDatasetActionOutputTypeDef

```python
# SqlQueryDatasetActionOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SqlQueryDatasetActionOutputTypeDef


def get_value() -> SqlQueryDatasetActionOutputTypeDef:
    return {
        "sqlQuery": ...,
    }


# SqlQueryDatasetActionOutputTypeDef definition

class SqlQueryDatasetActionOutputTypeDef(TypedDict):
    sqlQuery: str,
    filters: NotRequired[List[QueryFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
## SqlQueryDatasetActionTypeDef

```python
# SqlQueryDatasetActionTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import SqlQueryDatasetActionTypeDef


def get_value() -> SqlQueryDatasetActionTypeDef:
    return {
        "sqlQuery": ...,
    }


# SqlQueryDatasetActionTypeDef definition

class SqlQueryDatasetActionTypeDef(TypedDict):
    sqlQuery: str,
    filters: NotRequired[Sequence[QueryFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
## DatasetContentDeliveryDestinationTypeDef

```python
# DatasetContentDeliveryDestinationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetContentDeliveryDestinationTypeDef


def get_value() -> DatasetContentDeliveryDestinationTypeDef:
    return {
        "iotEventsDestinationConfiguration": ...,
    }


# DatasetContentDeliveryDestinationTypeDef definition

class DatasetContentDeliveryDestinationTypeDef(TypedDict):
    iotEventsDestinationConfiguration: NotRequired[IotEventsDestinationConfigurationTypeDef],  # (1)
    s3DestinationConfiguration: NotRequired[S3DestinationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: IotEventsDestinationConfigurationTypeDef](./type_defs.md#ioteventsdestinationconfigurationtypedef) 
2. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## ContainerDatasetActionOutputTypeDef

```python
# ContainerDatasetActionOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ContainerDatasetActionOutputTypeDef


def get_value() -> ContainerDatasetActionOutputTypeDef:
    return {
        "image": ...,
    }


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
# ContainerDatasetActionTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ContainerDatasetActionTypeDef


def get_value() -> ContainerDatasetActionTypeDef:
    return {
        "image": ...,
    }


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
# PipelineTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import PipelineTypeDef


def get_value() -> PipelineTypeDef:
    return {
        "name": ...,
    }


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
# ListPipelinesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListPipelinesResponseTypeDef


def get_value() -> ListPipelinesResponseTypeDef:
    return {
        "pipelineSummaries": ...,
    }


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
# PipelineActivityTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import PipelineActivityTypeDef


def get_value() -> PipelineActivityTypeDef:
    return {
        "channel": ...,
    }


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
# DescribeChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribeChannelResponseTypeDef


def get_value() -> DescribeChannelResponseTypeDef:
    return {
        "channel": ...,
    }


# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    statistics: ChannelStatisticsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ChannelStatisticsTypeDef](./type_defs.md#channelstatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelRequestTypeDef

```python
# CreateChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateChannelRequestTypeDef


def get_value() -> CreateChannelRequestTypeDef:
    return {
        "channelName": ...,
    }


# CreateChannelRequestTypeDef definition

class CreateChannelRequestTypeDef(TypedDict):
    channelName: str,
    channelStorage: NotRequired[ChannelStorageUnionTypeDef],  # (1)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef) [:material-code-braces: ChannelStorageOutputTypeDef](./type_defs.md#channelstorageoutputtypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateChannelRequestTypeDef

```python
# UpdateChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import UpdateChannelRequestTypeDef


def get_value() -> UpdateChannelRequestTypeDef:
    return {
        "channelName": ...,
    }


# UpdateChannelRequestTypeDef definition

class UpdateChannelRequestTypeDef(TypedDict):
    channelName: str,
    channelStorage: NotRequired[ChannelStorageUnionTypeDef],  # (1)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef) [:material-code-braces: ChannelStorageOutputTypeDef](./type_defs.md#channelstorageoutputtypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListChannelsResponseTypeDef


def get_value() -> ListChannelsResponseTypeDef:
    return {
        "channelSummaries": ...,
    }


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
# FileFormatConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import FileFormatConfigurationOutputTypeDef


def get_value() -> FileFormatConfigurationOutputTypeDef:
    return {
        "jsonConfiguration": ...,
    }


# FileFormatConfigurationOutputTypeDef definition

class FileFormatConfigurationOutputTypeDef(TypedDict):
    jsonConfiguration: NotRequired[Dict[str, Any]],
    parquetConfiguration: NotRequired[ParquetConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ParquetConfigurationOutputTypeDef](./type_defs.md#parquetconfigurationoutputtypedef) 
## FileFormatConfigurationTypeDef

```python
# FileFormatConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import FileFormatConfigurationTypeDef


def get_value() -> FileFormatConfigurationTypeDef:
    return {
        "jsonConfiguration": ...,
    }


# FileFormatConfigurationTypeDef definition

class FileFormatConfigurationTypeDef(TypedDict):
    jsonConfiguration: NotRequired[Mapping[str, Any]],
    parquetConfiguration: NotRequired[ParquetConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ParquetConfigurationTypeDef](./type_defs.md#parquetconfigurationtypedef) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatasetsResponseTypeDef


def get_value() -> ListDatasetsResponseTypeDef:
    return {
        "datasetSummaries": ...,
    }


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
# DatastoreSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreSummaryTypeDef


def get_value() -> DatastoreSummaryTypeDef:
    return {
        "datastoreName": ...,
    }


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
# DatasetContentDeliveryRuleTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetContentDeliveryRuleTypeDef


def get_value() -> DatasetContentDeliveryRuleTypeDef:
    return {
        "entryName": ...,
    }


# DatasetContentDeliveryRuleTypeDef definition

class DatasetContentDeliveryRuleTypeDef(TypedDict):
    destination: DatasetContentDeliveryDestinationTypeDef,  # (1)
    entryName: NotRequired[str],
```

1. See [:material-code-braces: DatasetContentDeliveryDestinationTypeDef](./type_defs.md#datasetcontentdeliverydestinationtypedef) 
## DatasetActionOutputTypeDef

```python
# DatasetActionOutputTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetActionOutputTypeDef


def get_value() -> DatasetActionOutputTypeDef:
    return {
        "actionName": ...,
    }


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
# DescribePipelineResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribePipelineResponseTypeDef


def get_value() -> DescribePipelineResponseTypeDef:
    return {
        "pipeline": ...,
    }


# DescribePipelineResponseTypeDef definition

class DescribePipelineResponseTypeDef(TypedDict):
    pipeline: PipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatastoreTypeDef

```python
# DatastoreTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatastoreTypeDef


def get_value() -> DatastoreTypeDef:
    return {
        "name": ...,
    }


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
# ListDatastoresResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import ListDatastoresResponseTypeDef


def get_value() -> ListDatastoresResponseTypeDef:
    return {
        "datastoreSummaries": ...,
    }


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
# DatasetTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetTypeDef


def get_value() -> DatasetTypeDef:
    return {
        "name": ...,
    }


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
# DatasetActionTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DatasetActionTypeDef


def get_value() -> DatasetActionTypeDef:
    return {
        "actionName": ...,
    }


# DatasetActionTypeDef definition

class DatasetActionTypeDef(TypedDict):
    actionName: NotRequired[str],
    queryAction: NotRequired[SqlQueryDatasetActionUnionTypeDef],  # (1)
    containerAction: NotRequired[ContainerDatasetActionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: SqlQueryDatasetActionTypeDef](./type_defs.md#sqlquerydatasetactiontypedef) [:material-code-braces: SqlQueryDatasetActionOutputTypeDef](./type_defs.md#sqlquerydatasetactionoutputtypedef) 
2. See [:material-code-braces: ContainerDatasetActionTypeDef](./type_defs.md#containerdatasetactiontypedef) [:material-code-braces: ContainerDatasetActionOutputTypeDef](./type_defs.md#containerdatasetactionoutputtypedef) 
## CreatePipelineRequestTypeDef

```python
# CreatePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreatePipelineRequestTypeDef


def get_value() -> CreatePipelineRequestTypeDef:
    return {
        "pipelineName": ...,
    }


# CreatePipelineRequestTypeDef definition

class CreatePipelineRequestTypeDef(TypedDict):
    pipelineName: str,
    pipelineActivities: Sequence[PipelineActivityUnionTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RunPipelineActivityRequestTypeDef

```python
# RunPipelineActivityRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import RunPipelineActivityRequestTypeDef


def get_value() -> RunPipelineActivityRequestTypeDef:
    return {
        "pipelineActivity": ...,
    }


# RunPipelineActivityRequestTypeDef definition

class RunPipelineActivityRequestTypeDef(TypedDict):
    pipelineActivity: PipelineActivityUnionTypeDef,  # (1)
    payloads: Sequence[BlobTypeDef],
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
## UpdatePipelineRequestTypeDef

```python
# UpdatePipelineRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import UpdatePipelineRequestTypeDef


def get_value() -> UpdatePipelineRequestTypeDef:
    return {
        "pipelineName": ...,
    }


# UpdatePipelineRequestTypeDef definition

class UpdatePipelineRequestTypeDef(TypedDict):
    pipelineName: str,
    pipelineActivities: Sequence[PipelineActivityUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
## DescribeDatastoreResponseTypeDef

```python
# DescribeDatastoreResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribeDatastoreResponseTypeDef


def get_value() -> DescribeDatastoreResponseTypeDef:
    return {
        "datastore": ...,
    }


# DescribeDatastoreResponseTypeDef definition

class DescribeDatastoreResponseTypeDef(TypedDict):
    datastore: DatastoreTypeDef,  # (1)
    statistics: DatastoreStatisticsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DatastoreTypeDef](./type_defs.md#datastoretypedef) 
2. See [:material-code-braces: DatastoreStatisticsTypeDef](./type_defs.md#datastorestatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatastoreRequestTypeDef

```python
# CreateDatastoreRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateDatastoreRequestTypeDef


def get_value() -> CreateDatastoreRequestTypeDef:
    return {
        "datastoreName": ...,
    }


# CreateDatastoreRequestTypeDef definition

class CreateDatastoreRequestTypeDef(TypedDict):
    datastoreName: str,
    datastoreStorage: NotRequired[DatastoreStorageUnionTypeDef],  # (1)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    fileFormatConfiguration: NotRequired[FileFormatConfigurationUnionTypeDef],  # (4)
    datastorePartitions: NotRequired[DatastorePartitionsUnionTypeDef],  # (5)
```

1. See [:material-code-braces: DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef) [:material-code-braces: DatastoreStorageOutputTypeDef](./type_defs.md#datastorestorageoutputtypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef) [:material-code-braces: FileFormatConfigurationOutputTypeDef](./type_defs.md#fileformatconfigurationoutputtypedef) 
5. See [:material-code-braces: DatastorePartitionsTypeDef](./type_defs.md#datastorepartitionstypedef) [:material-code-braces: DatastorePartitionsOutputTypeDef](./type_defs.md#datastorepartitionsoutputtypedef) 
## UpdateDatastoreRequestTypeDef

```python
# UpdateDatastoreRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import UpdateDatastoreRequestTypeDef


def get_value() -> UpdateDatastoreRequestTypeDef:
    return {
        "datastoreName": ...,
    }


# UpdateDatastoreRequestTypeDef definition

class UpdateDatastoreRequestTypeDef(TypedDict):
    datastoreName: str,
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (1)
    datastoreStorage: NotRequired[DatastoreStorageUnionTypeDef],  # (2)
    fileFormatConfiguration: NotRequired[FileFormatConfigurationUnionTypeDef],  # (3)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef) [:material-code-braces: DatastoreStorageOutputTypeDef](./type_defs.md#datastorestorageoutputtypedef) 
3. See [:material-code-braces: FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef) [:material-code-braces: FileFormatConfigurationOutputTypeDef](./type_defs.md#fileformatconfigurationoutputtypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import DescribeDatasetResponseTypeDef


def get_value() -> DescribeDatasetResponseTypeDef:
    return {
        "dataset": ...,
    }


# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    dataset: DatasetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetRequestTypeDef

```python
# CreateDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import CreateDatasetRequestTypeDef


def get_value() -> CreateDatasetRequestTypeDef:
    return {
        "datasetName": ...,
    }


# CreateDatasetRequestTypeDef definition

class CreateDatasetRequestTypeDef(TypedDict):
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
## UpdateDatasetRequestTypeDef

```python
# UpdateDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotanalytics.type_defs import UpdateDatasetRequestTypeDef


def get_value() -> UpdateDatasetRequestTypeDef:
    return {
        "datasetName": ...,
    }


# UpdateDatasetRequestTypeDef definition

class UpdateDatasetRequestTypeDef(TypedDict):
    datasetName: str,
    actions: Sequence[DatasetActionUnionTypeDef],  # (1)
    triggers: NotRequired[Sequence[DatasetTriggerTypeDef]],  # (2)
    contentDeliveryRules: NotRequired[Sequence[DatasetContentDeliveryRuleTypeDef]],  # (3)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (4)
    versioningConfiguration: NotRequired[VersioningConfigurationTypeDef],  # (5)
    lateDataRules: NotRequired[Sequence[LateDataRuleTypeDef]],  # (6)
```

1. See [:material-code-braces: DatasetActionTypeDef](./type_defs.md#datasetactiontypedef) [:material-code-braces: DatasetActionOutputTypeDef](./type_defs.md#datasetactionoutputtypedef) 
2. See [:material-code-braces: DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef) 
3. See [:material-code-braces: DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
6. See [:material-code-braces: LateDataRuleTypeDef](./type_defs.md#latedataruletypedef) 
