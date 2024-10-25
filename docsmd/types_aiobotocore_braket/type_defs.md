# Type definitions

> [Index](../README.md) > [Braket](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
    type annotations stubs module [types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).



## ContainerImageTypeDef

```python
# ContainerImageTypeDef definition

class ContainerImageTypeDef(TypedDict):
    uri: str,
```

## ScriptModeConfigTypeDef

```python
# ScriptModeConfigTypeDef definition

class ScriptModeConfigTypeDef(TypedDict):
    entryPoint: str,
    s3Uri: str,
    compressionType: NotRequired[CompressionTypeType],  # (1)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
## AssociationTypeDef

```python
# AssociationTypeDef definition

class AssociationTypeDef(TypedDict):
    arn: str,
    type: AssociationTypeType,  # (1)
```

1. See [:material-code-brackets: AssociationTypeType](./literals.md#associationtypetype) 
## CancelJobRequestRequestTypeDef

```python
# CancelJobRequestRequestTypeDef definition

class CancelJobRequestRequestTypeDef(TypedDict):
    jobArn: str,
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

## CancelQuantumTaskRequestRequestTypeDef

```python
# CancelQuantumTaskRequestRequestTypeDef definition

class CancelQuantumTaskRequestRequestTypeDef(TypedDict):
    clientToken: str,
    quantumTaskArn: str,
```

## DeviceConfigTypeDef

```python
# DeviceConfigTypeDef definition

class DeviceConfigTypeDef(TypedDict):
    device: str,
```

## InstanceConfigTypeDef

```python
# InstanceConfigTypeDef definition

class InstanceConfigTypeDef(TypedDict):
    instanceType: InstanceTypeType,  # (1)
    volumeSizeInGb: int,
    instanceCount: NotRequired[int],
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## JobCheckpointConfigTypeDef

```python
# JobCheckpointConfigTypeDef definition

class JobCheckpointConfigTypeDef(TypedDict):
    s3Uri: str,
    localPath: NotRequired[str],
```

## JobOutputDataConfigTypeDef

```python
# JobOutputDataConfigTypeDef definition

class JobOutputDataConfigTypeDef(TypedDict):
    s3Path: str,
    kmsKeyId: NotRequired[str],
```

## JobStoppingConditionTypeDef

```python
# JobStoppingConditionTypeDef definition

class JobStoppingConditionTypeDef(TypedDict):
    maxRuntimeInSeconds: NotRequired[int],
```

## S3DataSourceTypeDef

```python
# S3DataSourceTypeDef definition

class S3DataSourceTypeDef(TypedDict):
    s3Uri: str,
```

## DeviceQueueInfoTypeDef

```python
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
## GetDeviceRequestRequestTypeDef

```python
# GetDeviceRequestRequestTypeDef definition

class GetDeviceRequestRequestTypeDef(TypedDict):
    deviceArn: str,
```

## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    jobArn: str,
    additionalAttributeNames: NotRequired[Sequence[HybridJobAdditionalAttributeNameType]],  # (1)
```

1. See [:material-code-brackets: HybridJobAdditionalAttributeNameType](./literals.md#hybridjobadditionalattributenametype) 
## HybridJobQueueInfoTypeDef

```python
# HybridJobQueueInfoTypeDef definition

class HybridJobQueueInfoTypeDef(TypedDict):
    position: str,
    queue: QueueNameType,  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: QueueNameType](./literals.md#queuenametype) 
## JobEventDetailsTypeDef

```python
# JobEventDetailsTypeDef definition

class JobEventDetailsTypeDef(TypedDict):
    eventType: NotRequired[JobEventTypeType],  # (1)
    message: NotRequired[str],
    timeOfEvent: NotRequired[datetime],
```

1. See [:material-code-brackets: JobEventTypeType](./literals.md#jobeventtypetype) 
## GetQuantumTaskRequestRequestTypeDef

```python
# GetQuantumTaskRequestRequestTypeDef definition

class GetQuantumTaskRequestRequestTypeDef(TypedDict):
    quantumTaskArn: str,
    additionalAttributeNames: NotRequired[Sequence[QuantumTaskAdditionalAttributeNameType]],  # (1)
```

1. See [:material-code-brackets: QuantumTaskAdditionalAttributeNameType](./literals.md#quantumtaskadditionalattributenametype) 
## QuantumTaskQueueInfoTypeDef

```python
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
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## QuantumTaskSummaryTypeDef

```python
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
# SearchDevicesFilterTypeDef definition

class SearchDevicesFilterTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
```

## SearchJobsFilterTypeDef

```python
# SearchJobsFilterTypeDef definition

class SearchJobsFilterTypeDef(TypedDict):
    name: str,
    operator: SearchJobsFilterOperatorType,  # (1)
    values: Sequence[str],
```

1. See [:material-code-brackets: SearchJobsFilterOperatorType](./literals.md#searchjobsfilteroperatortype) 
## SearchQuantumTasksFilterTypeDef

```python
# SearchQuantumTasksFilterTypeDef definition

class SearchQuantumTasksFilterTypeDef(TypedDict):
    name: str,
    operator: SearchQuantumTasksFilterOperatorType,  # (1)
    values: Sequence[str],
```

1. See [:material-code-brackets: SearchQuantumTasksFilterOperatorType](./literals.md#searchquantumtasksfilteroperatortype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AlgorithmSpecificationTypeDef

```python
# AlgorithmSpecificationTypeDef definition

class AlgorithmSpecificationTypeDef(TypedDict):
    containerImage: NotRequired[ContainerImageTypeDef],  # (1)
    scriptModeConfig: NotRequired[ScriptModeConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ContainerImageTypeDef](./type_defs.md#containerimagetypedef) 
2. See [:material-code-braces: ScriptModeConfigTypeDef](./type_defs.md#scriptmodeconfigtypedef) 
## CreateQuantumTaskRequestRequestTypeDef

```python
# CreateQuantumTaskRequestRequestTypeDef definition

class CreateQuantumTaskRequestRequestTypeDef(TypedDict):
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
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQuantumTaskResponseTypeDef

```python
# CreateQuantumTaskResponseTypeDef definition

class CreateQuantumTaskResponseTypeDef(TypedDict):
    quantumTaskArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    s3DataSource: S3DataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef) 
## GetDeviceResponseTypeDef

```python
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
# SearchQuantumTasksResponseTypeDef definition

class SearchQuantumTasksResponseTypeDef(TypedDict):
    quantumTasks: List[QuantumTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QuantumTaskSummaryTypeDef](./type_defs.md#quantumtasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchDevicesRequestRequestTypeDef

```python
# SearchDevicesRequestRequestTypeDef definition

class SearchDevicesRequestRequestTypeDef(TypedDict):
    filters: Sequence[SearchDevicesFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef) 
## SearchDevicesRequestSearchDevicesPaginateTypeDef

```python
# SearchDevicesRequestSearchDevicesPaginateTypeDef definition

class SearchDevicesRequestSearchDevicesPaginateTypeDef(TypedDict):
    filters: Sequence[SearchDevicesFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchJobsRequestRequestTypeDef

```python
# SearchJobsRequestRequestTypeDef definition

class SearchJobsRequestRequestTypeDef(TypedDict):
    filters: Sequence[SearchJobsFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef) 
## SearchJobsRequestSearchJobsPaginateTypeDef

```python
# SearchJobsRequestSearchJobsPaginateTypeDef definition

class SearchJobsRequestSearchJobsPaginateTypeDef(TypedDict):
    filters: Sequence[SearchJobsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchQuantumTasksRequestRequestTypeDef

```python
# SearchQuantumTasksRequestRequestTypeDef definition

class SearchQuantumTasksRequestRequestTypeDef(TypedDict):
    filters: Sequence[SearchQuantumTasksFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef) 
## SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef

```python
# SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef definition

class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(TypedDict):
    filters: Sequence[SearchQuantumTasksFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## InputFileConfigTypeDef

```python
# InputFileConfigTypeDef definition

class InputFileConfigTypeDef(TypedDict):
    channelName: str,
    dataSource: DataSourceTypeDef,  # (1)
    contentType: NotRequired[str],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
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
