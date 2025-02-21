# Type definitions

> [Index](../README.md) > [Braket](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#braket)
    type annotations stubs module [types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).



## ContainerImageTypeDef

```python
# ContainerImageTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import ContainerImageTypeDef


def get_value() -> ContainerImageTypeDef:
    return {
        "uri": ...,
    }


# ContainerImageTypeDef definition

class ContainerImageTypeDef(TypedDict):
    uri: str,
```

## ScriptModeConfigTypeDef

```python
# ScriptModeConfigTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import ScriptModeConfigTypeDef


def get_value() -> ScriptModeConfigTypeDef:
    return {
        "compressionType": ...,
    }


# ScriptModeConfigTypeDef definition

class ScriptModeConfigTypeDef(TypedDict):
    entryPoint: str,
    s3Uri: str,
    compressionType: NotRequired[CompressionTypeType],  # (1)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
## AssociationTypeDef

```python
# AssociationTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import AssociationTypeDef


def get_value() -> AssociationTypeDef:
    return {
        "arn": ...,
    }


# AssociationTypeDef definition

class AssociationTypeDef(TypedDict):
    arn: str,
    type: AssociationTypeType,  # (1)
```

1. See [:material-code-brackets: AssociationTypeType](./literals.md#associationtypetype) 
## CancelJobRequestTypeDef

```python
# CancelJobRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CancelJobRequestTypeDef


def get_value() -> CancelJobRequestTypeDef:
    return {
        "jobArn": ...,
    }


# CancelJobRequestTypeDef definition

class CancelJobRequestTypeDef(TypedDict):
    jobArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import ResponseMetadataTypeDef


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

## CancelQuantumTaskRequestTypeDef

```python
# CancelQuantumTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CancelQuantumTaskRequestTypeDef


def get_value() -> CancelQuantumTaskRequestTypeDef:
    return {
        "clientToken": ...,
    }


# CancelQuantumTaskRequestTypeDef definition

class CancelQuantumTaskRequestTypeDef(TypedDict):
    clientToken: str,
    quantumTaskArn: str,
```

## DeviceConfigTypeDef

```python
# DeviceConfigTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import DeviceConfigTypeDef


def get_value() -> DeviceConfigTypeDef:
    return {
        "device": ...,
    }


# DeviceConfigTypeDef definition

class DeviceConfigTypeDef(TypedDict):
    device: str,
```

## InstanceConfigTypeDef

```python
# InstanceConfigTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import InstanceConfigTypeDef


def get_value() -> InstanceConfigTypeDef:
    return {
        "instanceCount": ...,
    }


# InstanceConfigTypeDef definition

class InstanceConfigTypeDef(TypedDict):
    instanceType: InstanceTypeType,  # (1)
    volumeSizeInGb: int,
    instanceCount: NotRequired[int],
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## JobCheckpointConfigTypeDef

```python
# JobCheckpointConfigTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import JobCheckpointConfigTypeDef


def get_value() -> JobCheckpointConfigTypeDef:
    return {
        "localPath": ...,
    }


# JobCheckpointConfigTypeDef definition

class JobCheckpointConfigTypeDef(TypedDict):
    s3Uri: str,
    localPath: NotRequired[str],
```

## JobOutputDataConfigTypeDef

```python
# JobOutputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import JobOutputDataConfigTypeDef


def get_value() -> JobOutputDataConfigTypeDef:
    return {
        "kmsKeyId": ...,
    }


# JobOutputDataConfigTypeDef definition

class JobOutputDataConfigTypeDef(TypedDict):
    s3Path: str,
    kmsKeyId: NotRequired[str],
```

## JobStoppingConditionTypeDef

```python
# JobStoppingConditionTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import JobStoppingConditionTypeDef


def get_value() -> JobStoppingConditionTypeDef:
    return {
        "maxRuntimeInSeconds": ...,
    }


# JobStoppingConditionTypeDef definition

class JobStoppingConditionTypeDef(TypedDict):
    maxRuntimeInSeconds: NotRequired[int],
```

## S3DataSourceTypeDef

```python
# S3DataSourceTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import S3DataSourceTypeDef


def get_value() -> S3DataSourceTypeDef:
    return {
        "s3Uri": ...,
    }


# S3DataSourceTypeDef definition

class S3DataSourceTypeDef(TypedDict):
    s3Uri: str,
```

## DeviceQueueInfoTypeDef

```python
# DeviceQueueInfoTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import DeviceQueueInfoTypeDef


def get_value() -> DeviceQueueInfoTypeDef:
    return {
        "queue": ...,
    }


# DeviceQueueInfoTypeDef definition

class DeviceQueueInfoTypeDef(TypedDict):
    queue: QueueNameType,  # (1)
    queueSize: str,
    queuePriority: NotRequired[QueuePriorityType],  # (2)
```

1. See [:material-code-brackets: QueueNameType](./literals.md#queuenametype) 
2. See [:material-code-brackets: QueuePriorityType](./literals.md#queueprioritytype) 
## DeviceSummaryTypeDef

```python
# DeviceSummaryTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import DeviceSummaryTypeDef


def get_value() -> DeviceSummaryTypeDef:
    return {
        "deviceArn": ...,
    }


# DeviceSummaryTypeDef definition

class DeviceSummaryTypeDef(TypedDict):
    deviceArn: str,
    deviceName: str,
    deviceStatus: DeviceStatusType,  # (1)
    deviceType: DeviceTypeType,  # (2)
    providerName: str,
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
2. See [:material-code-brackets: DeviceTypeType](./literals.md#devicetypetype) 
## GetDeviceRequestTypeDef

```python
# GetDeviceRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import GetDeviceRequestTypeDef


def get_value() -> GetDeviceRequestTypeDef:
    return {
        "deviceArn": ...,
    }


# GetDeviceRequestTypeDef definition

class GetDeviceRequestTypeDef(TypedDict):
    deviceArn: str,
```

## GetJobRequestTypeDef

```python
# GetJobRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import GetJobRequestTypeDef


def get_value() -> GetJobRequestTypeDef:
    return {
        "jobArn": ...,
    }


# GetJobRequestTypeDef definition

class GetJobRequestTypeDef(TypedDict):
    jobArn: str,
    additionalAttributeNames: NotRequired[Sequence[HybridJobAdditionalAttributeNameType]],  # (1)
```

1. See [:material-code-brackets: HybridJobAdditionalAttributeNameType](./literals.md#hybridjobadditionalattributenametype) 
## HybridJobQueueInfoTypeDef

```python
# HybridJobQueueInfoTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import HybridJobQueueInfoTypeDef


def get_value() -> HybridJobQueueInfoTypeDef:
    return {
        "message": ...,
    }


# HybridJobQueueInfoTypeDef definition

class HybridJobQueueInfoTypeDef(TypedDict):
    position: str,
    queue: QueueNameType,  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: QueueNameType](./literals.md#queuenametype) 
## JobEventDetailsTypeDef

```python
# JobEventDetailsTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import JobEventDetailsTypeDef


def get_value() -> JobEventDetailsTypeDef:
    return {
        "eventType": ...,
    }


# JobEventDetailsTypeDef definition

class JobEventDetailsTypeDef(TypedDict):
    eventType: NotRequired[JobEventTypeType],  # (1)
    message: NotRequired[str],
    timeOfEvent: NotRequired[datetime],
```

1. See [:material-code-brackets: JobEventTypeType](./literals.md#jobeventtypetype) 
## GetQuantumTaskRequestTypeDef

```python
# GetQuantumTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import GetQuantumTaskRequestTypeDef


def get_value() -> GetQuantumTaskRequestTypeDef:
    return {
        "quantumTaskArn": ...,
    }


# GetQuantumTaskRequestTypeDef definition

class GetQuantumTaskRequestTypeDef(TypedDict):
    quantumTaskArn: str,
    additionalAttributeNames: NotRequired[Sequence[QuantumTaskAdditionalAttributeNameType]],  # (1)
```

1. See [:material-code-brackets: QuantumTaskAdditionalAttributeNameType](./literals.md#quantumtaskadditionalattributenametype) 
## QuantumTaskQueueInfoTypeDef

```python
# QuantumTaskQueueInfoTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import QuantumTaskQueueInfoTypeDef


def get_value() -> QuantumTaskQueueInfoTypeDef:
    return {
        "message": ...,
    }


# QuantumTaskQueueInfoTypeDef definition

class QuantumTaskQueueInfoTypeDef(TypedDict):
    position: str,
    queue: QueueNameType,  # (1)
    message: NotRequired[str],
    queuePriority: NotRequired[QueuePriorityType],  # (2)
```

1. See [:material-code-brackets: QueueNameType](./literals.md#queuenametype) 
2. See [:material-code-brackets: QueuePriorityType](./literals.md#queueprioritytype) 
## JobSummaryTypeDef

```python
# JobSummaryTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import JobSummaryTypeDef


def get_value() -> JobSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    createdAt: datetime,
    device: str,
    jobArn: str,
    jobName: str,
    status: JobPrimaryStatusType,  # (1)
    endedAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: JobPrimaryStatusType](./literals.md#jobprimarystatustype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import PaginatorConfigTypeDef


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

## QuantumTaskSummaryTypeDef

```python
# QuantumTaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import QuantumTaskSummaryTypeDef


def get_value() -> QuantumTaskSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# QuantumTaskSummaryTypeDef definition

class QuantumTaskSummaryTypeDef(TypedDict):
    createdAt: datetime,
    deviceArn: str,
    outputS3Bucket: str,
    outputS3Directory: str,
    quantumTaskArn: str,
    shots: int,
    status: QuantumTaskStatusType,  # (1)
    endedAt: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: QuantumTaskStatusType](./literals.md#quantumtaskstatustype) 
## SearchDevicesFilterTypeDef

```python
# SearchDevicesFilterTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchDevicesFilterTypeDef


def get_value() -> SearchDevicesFilterTypeDef:
    return {
        "name": ...,
    }


# SearchDevicesFilterTypeDef definition

class SearchDevicesFilterTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
```

## SearchJobsFilterTypeDef

```python
# SearchJobsFilterTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchJobsFilterTypeDef


def get_value() -> SearchJobsFilterTypeDef:
    return {
        "name": ...,
    }


# SearchJobsFilterTypeDef definition

class SearchJobsFilterTypeDef(TypedDict):
    name: str,
    operator: SearchJobsFilterOperatorType,  # (1)
    values: Sequence[str],
```

1. See [:material-code-brackets: SearchJobsFilterOperatorType](./literals.md#searchjobsfilteroperatortype) 
## SearchQuantumTasksFilterTypeDef

```python
# SearchQuantumTasksFilterTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchQuantumTasksFilterTypeDef


def get_value() -> SearchQuantumTasksFilterTypeDef:
    return {
        "name": ...,
    }


# SearchQuantumTasksFilterTypeDef definition

class SearchQuantumTasksFilterTypeDef(TypedDict):
    name: str,
    operator: SearchQuantumTasksFilterOperatorType,  # (1)
    values: Sequence[str],
```

1. See [:material-code-brackets: SearchQuantumTasksFilterOperatorType](./literals.md#searchquantumtasksfilteroperatortype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AlgorithmSpecificationTypeDef

```python
# AlgorithmSpecificationTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import AlgorithmSpecificationTypeDef


def get_value() -> AlgorithmSpecificationTypeDef:
    return {
        "containerImage": ...,
    }


# AlgorithmSpecificationTypeDef definition

class AlgorithmSpecificationTypeDef(TypedDict):
    containerImage: NotRequired[ContainerImageTypeDef],  # (1)
    scriptModeConfig: NotRequired[ScriptModeConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ContainerImageTypeDef](./type_defs.md#containerimagetypedef) 
2. See [:material-code-braces: ScriptModeConfigTypeDef](./type_defs.md#scriptmodeconfigtypedef) 
## CreateQuantumTaskRequestTypeDef

```python
# CreateQuantumTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CreateQuantumTaskRequestTypeDef


def get_value() -> CreateQuantumTaskRequestTypeDef:
    return {
        "action": ...,
    }


# CreateQuantumTaskRequestTypeDef definition

class CreateQuantumTaskRequestTypeDef(TypedDict):
    action: str,
    clientToken: str,
    deviceArn: str,
    outputS3Bucket: str,
    outputS3KeyPrefix: str,
    shots: int,
    associations: NotRequired[Sequence[AssociationTypeDef]],  # (1)
    deviceParameters: NotRequired[str],
    jobToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AssociationTypeDef](./type_defs.md#associationtypedef) 
## CancelJobResponseTypeDef

```python
# CancelJobResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CancelJobResponseTypeDef


def get_value() -> CancelJobResponseTypeDef:
    return {
        "cancellationStatus": ...,
    }


# CancelJobResponseTypeDef definition

class CancelJobResponseTypeDef(TypedDict):
    cancellationStatus: CancellationStatusType,  # (1)
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CancellationStatusType](./literals.md#cancellationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelQuantumTaskResponseTypeDef

```python
# CancelQuantumTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CancelQuantumTaskResponseTypeDef


def get_value() -> CancelQuantumTaskResponseTypeDef:
    return {
        "cancellationStatus": ...,
    }


# CancelQuantumTaskResponseTypeDef definition

class CancelQuantumTaskResponseTypeDef(TypedDict):
    cancellationStatus: CancellationStatusType,  # (1)
    quantumTaskArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CancellationStatusType](./literals.md#cancellationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CreateJobResponseTypeDef


def get_value() -> CreateJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQuantumTaskResponseTypeDef

```python
# CreateQuantumTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CreateQuantumTaskResponseTypeDef


def get_value() -> CreateQuantumTaskResponseTypeDef:
    return {
        "quantumTaskArn": ...,
    }


# CreateQuantumTaskResponseTypeDef definition

class CreateQuantumTaskResponseTypeDef(TypedDict):
    quantumTaskArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import DataSourceTypeDef


def get_value() -> DataSourceTypeDef:
    return {
        "s3DataSource": ...,
    }


# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    s3DataSource: S3DataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef) 
## GetDeviceResponseTypeDef

```python
# GetDeviceResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import GetDeviceResponseTypeDef


def get_value() -> GetDeviceResponseTypeDef:
    return {
        "deviceArn": ...,
    }


# GetDeviceResponseTypeDef definition

class GetDeviceResponseTypeDef(TypedDict):
    deviceArn: str,
    deviceCapabilities: str,
    deviceName: str,
    deviceQueueInfo: List[DeviceQueueInfoTypeDef],  # (1)
    deviceStatus: DeviceStatusType,  # (2)
    deviceType: DeviceTypeType,  # (3)
    providerName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DeviceQueueInfoTypeDef](./type_defs.md#devicequeueinfotypedef) 
2. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
3. See [:material-code-brackets: DeviceTypeType](./literals.md#devicetypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchDevicesResponseTypeDef

```python
# SearchDevicesResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchDevicesResponseTypeDef


def get_value() -> SearchDevicesResponseTypeDef:
    return {
        "devices": ...,
    }


# SearchDevicesResponseTypeDef definition

class SearchDevicesResponseTypeDef(TypedDict):
    devices: List[DeviceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQuantumTaskResponseTypeDef

```python
# GetQuantumTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import GetQuantumTaskResponseTypeDef


def get_value() -> GetQuantumTaskResponseTypeDef:
    return {
        "associations": ...,
    }


# GetQuantumTaskResponseTypeDef definition

class GetQuantumTaskResponseTypeDef(TypedDict):
    associations: List[AssociationTypeDef],  # (1)
    createdAt: datetime,
    deviceArn: str,
    deviceParameters: str,
    endedAt: datetime,
    failureReason: str,
    jobArn: str,
    outputS3Bucket: str,
    outputS3Directory: str,
    quantumTaskArn: str,
    queueInfo: QuantumTaskQueueInfoTypeDef,  # (2)
    shots: int,
    status: QuantumTaskStatusType,  # (3)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AssociationTypeDef](./type_defs.md#associationtypedef) 
2. See [:material-code-braces: QuantumTaskQueueInfoTypeDef](./type_defs.md#quantumtaskqueueinfotypedef) 
3. See [:material-code-brackets: QuantumTaskStatusType](./literals.md#quantumtaskstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchJobsResponseTypeDef

```python
# SearchJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchJobsResponseTypeDef


def get_value() -> SearchJobsResponseTypeDef:
    return {
        "jobs": ...,
    }


# SearchJobsResponseTypeDef definition

class SearchJobsResponseTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchQuantumTasksResponseTypeDef

```python
# SearchQuantumTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchQuantumTasksResponseTypeDef


def get_value() -> SearchQuantumTasksResponseTypeDef:
    return {
        "nextToken": ...,
    }


# SearchQuantumTasksResponseTypeDef definition

class SearchQuantumTasksResponseTypeDef(TypedDict):
    quantumTasks: List[QuantumTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QuantumTaskSummaryTypeDef](./type_defs.md#quantumtasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchDevicesRequestPaginateTypeDef

```python
# SearchDevicesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchDevicesRequestPaginateTypeDef


def get_value() -> SearchDevicesRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# SearchDevicesRequestPaginateTypeDef definition

class SearchDevicesRequestPaginateTypeDef(TypedDict):
    filters: Sequence[SearchDevicesFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchDevicesRequestTypeDef

```python
# SearchDevicesRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchDevicesRequestTypeDef


def get_value() -> SearchDevicesRequestTypeDef:
    return {
        "filters": ...,
    }


# SearchDevicesRequestTypeDef definition

class SearchDevicesRequestTypeDef(TypedDict):
    filters: Sequence[SearchDevicesFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef) 
## SearchJobsRequestPaginateTypeDef

```python
# SearchJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchJobsRequestPaginateTypeDef


def get_value() -> SearchJobsRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# SearchJobsRequestPaginateTypeDef definition

class SearchJobsRequestPaginateTypeDef(TypedDict):
    filters: Sequence[SearchJobsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchJobsRequestTypeDef

```python
# SearchJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchJobsRequestTypeDef


def get_value() -> SearchJobsRequestTypeDef:
    return {
        "filters": ...,
    }


# SearchJobsRequestTypeDef definition

class SearchJobsRequestTypeDef(TypedDict):
    filters: Sequence[SearchJobsFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef) 
## SearchQuantumTasksRequestPaginateTypeDef

```python
# SearchQuantumTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchQuantumTasksRequestPaginateTypeDef


def get_value() -> SearchQuantumTasksRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# SearchQuantumTasksRequestPaginateTypeDef definition

class SearchQuantumTasksRequestPaginateTypeDef(TypedDict):
    filters: Sequence[SearchQuantumTasksFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchQuantumTasksRequestTypeDef

```python
# SearchQuantumTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import SearchQuantumTasksRequestTypeDef


def get_value() -> SearchQuantumTasksRequestTypeDef:
    return {
        "filters": ...,
    }


# SearchQuantumTasksRequestTypeDef definition

class SearchQuantumTasksRequestTypeDef(TypedDict):
    filters: Sequence[SearchQuantumTasksFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef) 
## InputFileConfigTypeDef

```python
# InputFileConfigTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import InputFileConfigTypeDef


def get_value() -> InputFileConfigTypeDef:
    return {
        "channelName": ...,
    }


# InputFileConfigTypeDef definition

class InputFileConfigTypeDef(TypedDict):
    channelName: str,
    dataSource: DataSourceTypeDef,  # (1)
    contentType: NotRequired[str],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## CreateJobRequestTypeDef

```python
# CreateJobRequestTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import CreateJobRequestTypeDef


def get_value() -> CreateJobRequestTypeDef:
    return {
        "algorithmSpecification": ...,
    }


# CreateJobRequestTypeDef definition

class CreateJobRequestTypeDef(TypedDict):
    algorithmSpecification: AlgorithmSpecificationTypeDef,  # (1)
    clientToken: str,
    deviceConfig: DeviceConfigTypeDef,  # (2)
    instanceConfig: InstanceConfigTypeDef,  # (3)
    jobName: str,
    outputDataConfig: JobOutputDataConfigTypeDef,  # (4)
    roleArn: str,
    associations: NotRequired[Sequence[AssociationTypeDef]],  # (5)
    checkpointConfig: NotRequired[JobCheckpointConfigTypeDef],  # (6)
    hyperParameters: NotRequired[Mapping[str, str]],
    inputDataConfig: NotRequired[Sequence[InputFileConfigTypeDef]],  # (7)
    stoppingCondition: NotRequired[JobStoppingConditionTypeDef],  # (8)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef) 
2. See [:material-code-braces: DeviceConfigTypeDef](./type_defs.md#deviceconfigtypedef) 
3. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
4. See [:material-code-braces: JobOutputDataConfigTypeDef](./type_defs.md#joboutputdataconfigtypedef) 
5. See [:material-code-braces: AssociationTypeDef](./type_defs.md#associationtypedef) 
6. See [:material-code-braces: JobCheckpointConfigTypeDef](./type_defs.md#jobcheckpointconfigtypedef) 
7. See [:material-code-braces: InputFileConfigTypeDef](./type_defs.md#inputfileconfigtypedef) 
8. See [:material-code-braces: JobStoppingConditionTypeDef](./type_defs.md#jobstoppingconditiontypedef) 
## GetJobResponseTypeDef

```python
# GetJobResponseTypeDef TypedDict usage example

from types_aiobotocore_braket.type_defs import GetJobResponseTypeDef


def get_value() -> GetJobResponseTypeDef:
    return {
        "algorithmSpecification": ...,
    }


# GetJobResponseTypeDef definition

class GetJobResponseTypeDef(TypedDict):
    algorithmSpecification: AlgorithmSpecificationTypeDef,  # (1)
    associations: List[AssociationTypeDef],  # (2)
    billableDuration: int,
    checkpointConfig: JobCheckpointConfigTypeDef,  # (3)
    createdAt: datetime,
    deviceConfig: DeviceConfigTypeDef,  # (4)
    endedAt: datetime,
    events: List[JobEventDetailsTypeDef],  # (5)
    failureReason: str,
    hyperParameters: Dict[str, str],
    inputDataConfig: List[InputFileConfigTypeDef],  # (6)
    instanceConfig: InstanceConfigTypeDef,  # (7)
    jobArn: str,
    jobName: str,
    outputDataConfig: JobOutputDataConfigTypeDef,  # (8)
    queueInfo: HybridJobQueueInfoTypeDef,  # (9)
    roleArn: str,
    startedAt: datetime,
    status: JobPrimaryStatusType,  # (10)
    stoppingCondition: JobStoppingConditionTypeDef,  # (11)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (12)
```

1. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef) 
2. See [:material-code-braces: AssociationTypeDef](./type_defs.md#associationtypedef) 
3. See [:material-code-braces: JobCheckpointConfigTypeDef](./type_defs.md#jobcheckpointconfigtypedef) 
4. See [:material-code-braces: DeviceConfigTypeDef](./type_defs.md#deviceconfigtypedef) 
5. See [:material-code-braces: JobEventDetailsTypeDef](./type_defs.md#jobeventdetailstypedef) 
6. See [:material-code-braces: InputFileConfigTypeDef](./type_defs.md#inputfileconfigtypedef) 
7. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
8. See [:material-code-braces: JobOutputDataConfigTypeDef](./type_defs.md#joboutputdataconfigtypedef) 
9. See [:material-code-braces: HybridJobQueueInfoTypeDef](./type_defs.md#hybridjobqueueinfotypedef) 
10. See [:material-code-brackets: JobPrimaryStatusType](./literals.md#jobprimarystatustype) 
11. See [:material-code-braces: JobStoppingConditionTypeDef](./type_defs.md#jobstoppingconditiontypedef) 
12. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
