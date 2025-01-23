# Type definitions

> [Index](../README.md) > [Omics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#omics)
    type annotations stubs module [types-aiobotocore-omics](https://pypi.org/project/types-aiobotocore-omics/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


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


## TsvStoreOptionsUnionTypeDef

```python
# TsvStoreOptionsUnionTypeDef definition

TsvStoreOptionsUnionTypeDef = Union[
    TsvStoreOptionsTypeDef,  # (1)
    TsvStoreOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TsvStoreOptionsTypeDef](./type_defs.md#tsvstoreoptionstypedef) 
2. See [:material-code-braces: TsvStoreOptionsOutputTypeDef](./type_defs.md#tsvstoreoptionsoutputtypedef) 

## TsvVersionOptionsUnionTypeDef

```python
# TsvVersionOptionsUnionTypeDef definition

TsvVersionOptionsUnionTypeDef = Union[
    TsvVersionOptionsTypeDef,  # (1)
    TsvVersionOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TsvVersionOptionsTypeDef](./type_defs.md#tsvversionoptionstypedef) 
2. See [:material-code-braces: TsvVersionOptionsOutputTypeDef](./type_defs.md#tsvversionoptionsoutputtypedef) 



## AbortMultipartReadSetUploadRequestRequestTypeDef

```python
# AbortMultipartReadSetUploadRequestRequestTypeDef definition

class AbortMultipartReadSetUploadRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    uploadId: str,
```

## AcceptShareRequestRequestTypeDef

```python
# AcceptShareRequestRequestTypeDef definition

class AcceptShareRequestRequestTypeDef(TypedDict):
    shareId: str,
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

## ActivateReadSetJobItemTypeDef

```python
# ActivateReadSetJobItemTypeDef definition

class ActivateReadSetJobItemTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    status: ReadSetActivationJobStatusType,  # (1)
    creationTime: datetime,
    completionTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReadSetActivationJobStatusType](./literals.md#readsetactivationjobstatustype) 
## ActivateReadSetSourceItemTypeDef

```python
# ActivateReadSetSourceItemTypeDef definition

class ActivateReadSetSourceItemTypeDef(TypedDict):
    readSetId: str,
    status: ReadSetActivationJobItemStatusType,  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ReadSetActivationJobItemStatusType](./literals.md#readsetactivationjobitemstatustype) 
## AnnotationImportItemDetailTypeDef

```python
# AnnotationImportItemDetailTypeDef definition

class AnnotationImportItemDetailTypeDef(TypedDict):
    source: str,
    jobStatus: JobStatusType,  # (1)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## AnnotationImportItemSourceTypeDef

```python
# AnnotationImportItemSourceTypeDef definition

class AnnotationImportItemSourceTypeDef(TypedDict):
    source: str,
```

## AnnotationImportJobItemTypeDef

```python
# AnnotationImportJobItemTypeDef definition

class AnnotationImportJobItemTypeDef(TypedDict):
    id: str,
    destinationName: str,
    versionName: str,
    roleArn: str,
    status: JobStatusType,  # (1)
    creationTime: datetime,
    updateTime: datetime,
    completionTime: NotRequired[datetime],
    runLeftNormalization: NotRequired[bool],
    annotationFields: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ReferenceItemTypeDef

```python
# ReferenceItemTypeDef definition

class ReferenceItemTypeDef(TypedDict):
    referenceArn: NotRequired[str],
```

## SseConfigTypeDef

```python
# SseConfigTypeDef definition

class SseConfigTypeDef(TypedDict):
    type: EncryptionTypeType,  # (1)
    keyArn: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## AnnotationStoreVersionItemTypeDef

```python
# AnnotationStoreVersionItemTypeDef definition

class AnnotationStoreVersionItemTypeDef(TypedDict):
    storeId: str,
    id: str,
    status: VersionStatusType,  # (1)
    versionArn: str,
    name: str,
    versionName: str,
    description: str,
    creationTime: datetime,
    updateTime: datetime,
    statusMessage: str,
    versionSizeBytes: int,
```

1. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
## BatchDeleteReadSetRequestRequestTypeDef

```python
# BatchDeleteReadSetRequestRequestTypeDef definition

class BatchDeleteReadSetRequestRequestTypeDef(TypedDict):
    ids: Sequence[str],
    sequenceStoreId: str,
```

## ReadSetBatchErrorTypeDef

```python
# ReadSetBatchErrorTypeDef definition

class ReadSetBatchErrorTypeDef(TypedDict):
    id: str,
    code: str,
    message: str,
```

## CancelAnnotationImportRequestRequestTypeDef

```python
# CancelAnnotationImportRequestRequestTypeDef definition

class CancelAnnotationImportRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## CancelRunRequestRequestTypeDef

```python
# CancelRunRequestRequestTypeDef definition

class CancelRunRequestRequestTypeDef(TypedDict):
    id: str,
```

## CancelVariantImportRequestRequestTypeDef

```python
# CancelVariantImportRequestRequestTypeDef definition

class CancelVariantImportRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## CompleteReadSetUploadPartListItemTypeDef

```python
# CompleteReadSetUploadPartListItemTypeDef definition

class CompleteReadSetUploadPartListItemTypeDef(TypedDict):
    partNumber: int,
    partSource: ReadSetPartSourceType,  # (1)
    checksum: str,
```

1. See [:material-code-brackets: ReadSetPartSourceType](./literals.md#readsetpartsourcetype) 
## CreateMultipartReadSetUploadRequestRequestTypeDef

```python
# CreateMultipartReadSetUploadRequestRequestTypeDef definition

class CreateMultipartReadSetUploadRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    sourceFileType: FileTypeType,  # (1)
    subjectId: str,
    sampleId: str,
    name: str,
    clientToken: NotRequired[str],
    generatedFrom: NotRequired[str],
    referenceArn: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
## CreateRunCacheRequestRequestTypeDef

```python
# CreateRunCacheRequestRequestTypeDef definition

class CreateRunCacheRequestRequestTypeDef(TypedDict):
    cacheS3Location: str,
    requestId: str,
    cacheBehavior: NotRequired[CacheBehaviorType],  # (1)
    description: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    cacheBucketOwnerId: NotRequired[str],
```

1. See [:material-code-brackets: CacheBehaviorType](./literals.md#cachebehaviortype) 
## CreateRunGroupRequestRequestTypeDef

```python
# CreateRunGroupRequestRequestTypeDef definition

class CreateRunGroupRequestRequestTypeDef(TypedDict):
    requestId: str,
    name: NotRequired[str],
    maxCpus: NotRequired[int],
    maxRuns: NotRequired[int],
    maxDuration: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
    maxGpus: NotRequired[int],
```

## S3AccessConfigTypeDef

```python
# S3AccessConfigTypeDef definition

class S3AccessConfigTypeDef(TypedDict):
    accessLogLocation: NotRequired[str],
```

## SequenceStoreS3AccessTypeDef

```python
# SequenceStoreS3AccessTypeDef definition

class SequenceStoreS3AccessTypeDef(TypedDict):
    s3Uri: NotRequired[str],
    s3AccessPointArn: NotRequired[str],
    accessLogLocation: NotRequired[str],
```

## CreateShareRequestRequestTypeDef

```python
# CreateShareRequestRequestTypeDef definition

class CreateShareRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    principalSubscriber: str,
    shareName: NotRequired[str],
```

## WorkflowParameterTypeDef

```python
# WorkflowParameterTypeDef definition

class WorkflowParameterTypeDef(TypedDict):
    description: NotRequired[str],
    optional: NotRequired[bool],
```

## DeleteAnnotationStoreRequestRequestTypeDef

```python
# DeleteAnnotationStoreRequestRequestTypeDef definition

class DeleteAnnotationStoreRequestRequestTypeDef(TypedDict):
    name: str,
    force: NotRequired[bool],
```

## DeleteAnnotationStoreVersionsRequestRequestTypeDef

```python
# DeleteAnnotationStoreVersionsRequestRequestTypeDef definition

class DeleteAnnotationStoreVersionsRequestRequestTypeDef(TypedDict):
    name: str,
    versions: Sequence[str],
    force: NotRequired[bool],
```

## VersionDeleteErrorTypeDef

```python
# VersionDeleteErrorTypeDef definition

class VersionDeleteErrorTypeDef(TypedDict):
    versionName: str,
    message: str,
```

## DeleteReferenceRequestRequestTypeDef

```python
# DeleteReferenceRequestRequestTypeDef definition

class DeleteReferenceRequestRequestTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
```

## DeleteReferenceStoreRequestRequestTypeDef

```python
# DeleteReferenceStoreRequestRequestTypeDef definition

class DeleteReferenceStoreRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteRunCacheRequestRequestTypeDef

```python
# DeleteRunCacheRequestRequestTypeDef definition

class DeleteRunCacheRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteRunGroupRequestRequestTypeDef

```python
# DeleteRunGroupRequestRequestTypeDef definition

class DeleteRunGroupRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteRunRequestRequestTypeDef

```python
# DeleteRunRequestRequestTypeDef definition

class DeleteRunRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteS3AccessPolicyRequestRequestTypeDef

```python
# DeleteS3AccessPolicyRequestRequestTypeDef definition

class DeleteS3AccessPolicyRequestRequestTypeDef(TypedDict):
    s3AccessPointArn: str,
```

## DeleteSequenceStoreRequestRequestTypeDef

```python
# DeleteSequenceStoreRequestRequestTypeDef definition

class DeleteSequenceStoreRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteShareRequestRequestTypeDef

```python
# DeleteShareRequestRequestTypeDef definition

class DeleteShareRequestRequestTypeDef(TypedDict):
    shareId: str,
```

## DeleteVariantStoreRequestRequestTypeDef

```python
# DeleteVariantStoreRequestRequestTypeDef definition

class DeleteVariantStoreRequestRequestTypeDef(TypedDict):
    name: str,
    force: NotRequired[bool],
```

## DeleteWorkflowRequestRequestTypeDef

```python
# DeleteWorkflowRequestRequestTypeDef definition

class DeleteWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
```

## ETagTypeDef

```python
# ETagTypeDef definition

class ETagTypeDef(TypedDict):
    algorithm: NotRequired[ETagAlgorithmType],  # (1)
    source1: NotRequired[str],
    source2: NotRequired[str],
```

1. See [:material-code-brackets: ETagAlgorithmType](./literals.md#etagalgorithmtype) 
## ExportReadSetDetailTypeDef

```python
# ExportReadSetDetailTypeDef definition

class ExportReadSetDetailTypeDef(TypedDict):
    id: str,
    status: ReadSetExportJobItemStatusType,  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ReadSetExportJobItemStatusType](./literals.md#readsetexportjobitemstatustype) 
## ExportReadSetJobDetailTypeDef

```python
# ExportReadSetJobDetailTypeDef definition

class ExportReadSetJobDetailTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    destination: str,
    status: ReadSetExportJobStatusType,  # (1)
    creationTime: datetime,
    completionTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReadSetExportJobStatusType](./literals.md#readsetexportjobstatustype) 
## ExportReadSetTypeDef

```python
# ExportReadSetTypeDef definition

class ExportReadSetTypeDef(TypedDict):
    readSetId: str,
```

## ReadSetS3AccessTypeDef

```python
# ReadSetS3AccessTypeDef definition

class ReadSetS3AccessTypeDef(TypedDict):
    s3Uri: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    resourceArns: NotRequired[Sequence[str]],
    status: NotRequired[Sequence[ShareStatusType]],  # (1)
    type: NotRequired[Sequence[ShareResourceTypeType]],  # (2)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-brackets: ShareResourceTypeType](./literals.md#shareresourcetypetype) 
## VcfOptionsTypeDef

```python
# VcfOptionsTypeDef definition

class VcfOptionsTypeDef(TypedDict):
    ignoreQualField: NotRequired[bool],
    ignoreFilterField: NotRequired[bool],
```

## GetAnnotationImportRequestRequestTypeDef

```python
# GetAnnotationImportRequestRequestTypeDef definition

class GetAnnotationImportRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetAnnotationStoreRequestRequestTypeDef

```python
# GetAnnotationStoreRequestRequestTypeDef definition

class GetAnnotationStoreRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetAnnotationStoreVersionRequestRequestTypeDef

```python
# GetAnnotationStoreVersionRequestRequestTypeDef definition

class GetAnnotationStoreVersionRequestRequestTypeDef(TypedDict):
    name: str,
    versionName: str,
```

## GetReadSetActivationJobRequestRequestTypeDef

```python
# GetReadSetActivationJobRequestRequestTypeDef definition

class GetReadSetActivationJobRequestRequestTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
```

## GetReadSetExportJobRequestRequestTypeDef

```python
# GetReadSetExportJobRequestRequestTypeDef definition

class GetReadSetExportJobRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    id: str,
```

## GetReadSetImportJobRequestRequestTypeDef

```python
# GetReadSetImportJobRequestRequestTypeDef definition

class GetReadSetImportJobRequestRequestTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
```

## GetReadSetMetadataRequestRequestTypeDef

```python
# GetReadSetMetadataRequestRequestTypeDef definition

class GetReadSetMetadataRequestRequestTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
```

## SequenceInformationTypeDef

```python
# SequenceInformationTypeDef definition

class SequenceInformationTypeDef(TypedDict):
    totalReadCount: NotRequired[int],
    totalBaseCount: NotRequired[int],
    generatedFrom: NotRequired[str],
    alignment: NotRequired[str],
```

## GetReadSetRequestRequestTypeDef

```python
# GetReadSetRequestRequestTypeDef definition

class GetReadSetRequestRequestTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    partNumber: int,
    file: NotRequired[ReadSetFileType],  # (1)
```

1. See [:material-code-brackets: ReadSetFileType](./literals.md#readsetfiletype) 
## GetReferenceImportJobRequestRequestTypeDef

```python
# GetReferenceImportJobRequestRequestTypeDef definition

class GetReferenceImportJobRequestRequestTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
```

## ImportReferenceSourceItemTypeDef

```python
# ImportReferenceSourceItemTypeDef definition

class ImportReferenceSourceItemTypeDef(TypedDict):
    status: ReferenceImportJobItemStatusType,  # (1)
    sourceFile: NotRequired[str],
    statusMessage: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    referenceId: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceImportJobItemStatusType](./literals.md#referenceimportjobitemstatustype) 
## GetReferenceMetadataRequestRequestTypeDef

```python
# GetReferenceMetadataRequestRequestTypeDef definition

class GetReferenceMetadataRequestRequestTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
```

## GetReferenceRequestRequestTypeDef

```python
# GetReferenceRequestRequestTypeDef definition

class GetReferenceRequestRequestTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
    partNumber: int,
    range: NotRequired[str],
    file: NotRequired[ReferenceFileType],  # (1)
```

1. See [:material-code-brackets: ReferenceFileType](./literals.md#referencefiletype) 
## GetReferenceStoreRequestRequestTypeDef

```python
# GetReferenceStoreRequestRequestTypeDef definition

class GetReferenceStoreRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetRunCacheRequestRequestTypeDef

```python
# GetRunCacheRequestRequestTypeDef definition

class GetRunCacheRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetRunGroupRequestRequestTypeDef

```python
# GetRunGroupRequestRequestTypeDef definition

class GetRunGroupRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetRunRequestRequestTypeDef

```python
# GetRunRequestRequestTypeDef definition

class GetRunRequestRequestTypeDef(TypedDict):
    id: str,
    export: NotRequired[Sequence[RunExportType]],  # (1)
```

1. See [:material-code-brackets: RunExportType](./literals.md#runexporttype) 
## RunLogLocationTypeDef

```python
# RunLogLocationTypeDef definition

class RunLogLocationTypeDef(TypedDict):
    engineLogStream: NotRequired[str],
    runLogStream: NotRequired[str],
```

## GetRunTaskRequestRequestTypeDef

```python
# GetRunTaskRequestRequestTypeDef definition

class GetRunTaskRequestRequestTypeDef(TypedDict):
    id: str,
    taskId: str,
```

## GetS3AccessPolicyRequestRequestTypeDef

```python
# GetS3AccessPolicyRequestRequestTypeDef definition

class GetS3AccessPolicyRequestRequestTypeDef(TypedDict):
    s3AccessPointArn: str,
```

## GetSequenceStoreRequestRequestTypeDef

```python
# GetSequenceStoreRequestRequestTypeDef definition

class GetSequenceStoreRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetShareRequestRequestTypeDef

```python
# GetShareRequestRequestTypeDef definition

class GetShareRequestRequestTypeDef(TypedDict):
    shareId: str,
```

## ShareDetailsTypeDef

```python
# ShareDetailsTypeDef definition

class ShareDetailsTypeDef(TypedDict):
    shareId: NotRequired[str],
    resourceArn: NotRequired[str],
    resourceId: NotRequired[str],
    principalSubscriber: NotRequired[str],
    ownerId: NotRequired[str],
    status: NotRequired[ShareStatusType],  # (1)
    statusMessage: NotRequired[str],
    shareName: NotRequired[str],
    creationTime: NotRequired[datetime],
    updateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## GetVariantImportRequestRequestTypeDef

```python
# GetVariantImportRequestRequestTypeDef definition

class GetVariantImportRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## VariantImportItemDetailTypeDef

```python
# VariantImportItemDetailTypeDef definition

class VariantImportItemDetailTypeDef(TypedDict):
    source: str,
    jobStatus: JobStatusType,  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## GetVariantStoreRequestRequestTypeDef

```python
# GetVariantStoreRequestRequestTypeDef definition

class GetVariantStoreRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetWorkflowRequestRequestTypeDef

```python
# GetWorkflowRequestRequestTypeDef definition

class GetWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
    type: NotRequired[WorkflowTypeType],  # (1)
    export: NotRequired[Sequence[WorkflowExportType]],  # (2)
    workflowOwnerId: NotRequired[str],
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: WorkflowExportType](./literals.md#workflowexporttype) 
## ImportReadSetJobItemTypeDef

```python
# ImportReadSetJobItemTypeDef definition

class ImportReadSetJobItemTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    roleArn: str,
    status: ReadSetImportJobStatusType,  # (1)
    creationTime: datetime,
    completionTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReadSetImportJobStatusType](./literals.md#readsetimportjobstatustype) 
## SourceFilesTypeDef

```python
# SourceFilesTypeDef definition

class SourceFilesTypeDef(TypedDict):
    source1: str,
    source2: NotRequired[str],
```

## ImportReferenceJobItemTypeDef

```python
# ImportReferenceJobItemTypeDef definition

class ImportReferenceJobItemTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
    roleArn: str,
    status: ReferenceImportJobStatusType,  # (1)
    creationTime: datetime,
    completionTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReferenceImportJobStatusType](./literals.md#referenceimportjobstatustype) 
## ListAnnotationImportJobsFilterTypeDef

```python
# ListAnnotationImportJobsFilterTypeDef definition

class ListAnnotationImportJobsFilterTypeDef(TypedDict):
    status: NotRequired[JobStatusType],  # (1)
    storeName: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAnnotationStoreVersionsFilterTypeDef

```python
# ListAnnotationStoreVersionsFilterTypeDef definition

class ListAnnotationStoreVersionsFilterTypeDef(TypedDict):
    status: NotRequired[VersionStatusType],  # (1)
```

1. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
## ListAnnotationStoresFilterTypeDef

```python
# ListAnnotationStoresFilterTypeDef definition

class ListAnnotationStoresFilterTypeDef(TypedDict):
    status: NotRequired[StoreStatusType],  # (1)
```

1. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
## ListMultipartReadSetUploadsRequestRequestTypeDef

```python
# ListMultipartReadSetUploadsRequestRequestTypeDef definition

class ListMultipartReadSetUploadsRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MultipartReadSetUploadListItemTypeDef

```python
# MultipartReadSetUploadListItemTypeDef definition

class MultipartReadSetUploadListItemTypeDef(TypedDict):
    sequenceStoreId: str,
    uploadId: str,
    sourceFileType: FileTypeType,  # (1)
    subjectId: str,
    sampleId: str,
    generatedFrom: str,
    referenceArn: str,
    creationTime: datetime,
    name: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
## ReadSetUploadPartListItemTypeDef

```python
# ReadSetUploadPartListItemTypeDef definition

class ReadSetUploadPartListItemTypeDef(TypedDict):
    partNumber: int,
    partSize: int,
    partSource: ReadSetPartSourceType,  # (1)
    checksum: str,
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReadSetPartSourceType](./literals.md#readsetpartsourcetype) 
## ReferenceListItemTypeDef

```python
# ReferenceListItemTypeDef definition

class ReferenceListItemTypeDef(TypedDict):
    id: str,
    arn: str,
    referenceStoreId: str,
    md5: str,
    creationTime: datetime,
    updateTime: datetime,
    status: NotRequired[ReferenceStatusType],  # (1)
    name: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceStatusType](./literals.md#referencestatustype) 
## ListRunCachesRequestRequestTypeDef

```python
# ListRunCachesRequestRequestTypeDef definition

class ListRunCachesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    startingToken: NotRequired[str],
```

## RunCacheListItemTypeDef

```python
# RunCacheListItemTypeDef definition

class RunCacheListItemTypeDef(TypedDict):
    arn: NotRequired[str],
    cacheBehavior: NotRequired[CacheBehaviorType],  # (1)
    cacheS3Uri: NotRequired[str],
    creationTime: NotRequired[datetime],
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[RunCacheStatusType],  # (2)
```

1. See [:material-code-brackets: CacheBehaviorType](./literals.md#cachebehaviortype) 
2. See [:material-code-brackets: RunCacheStatusType](./literals.md#runcachestatustype) 
## ListRunGroupsRequestRequestTypeDef

```python
# ListRunGroupsRequestRequestTypeDef definition

class ListRunGroupsRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    startingToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RunGroupListItemTypeDef

```python
# RunGroupListItemTypeDef definition

class RunGroupListItemTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    maxCpus: NotRequired[int],
    maxRuns: NotRequired[int],
    maxDuration: NotRequired[int],
    creationTime: NotRequired[datetime],
    maxGpus: NotRequired[int],
```

## ListRunTasksRequestRequestTypeDef

```python
# ListRunTasksRequestRequestTypeDef definition

class ListRunTasksRequestRequestTypeDef(TypedDict):
    id: str,
    status: NotRequired[TaskStatusType],  # (1)
    startingToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## TaskListItemTypeDef

```python
# TaskListItemTypeDef definition

class TaskListItemTypeDef(TypedDict):
    taskId: NotRequired[str],
    status: NotRequired[TaskStatusType],  # (1)
    name: NotRequired[str],
    cpus: NotRequired[int],
    cacheHit: NotRequired[bool],
    cacheS3Uri: NotRequired[str],
    memory: NotRequired[int],
    creationTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
    stopTime: NotRequired[datetime],
    gpus: NotRequired[int],
    instanceType: NotRequired[str],
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## ListRunsRequestRequestTypeDef

```python
# ListRunsRequestRequestTypeDef definition

class ListRunsRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    runGroupId: NotRequired[str],
    startingToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[RunStatusType],  # (1)
```

1. See [:material-code-brackets: RunStatusType](./literals.md#runstatustype) 
## RunListItemTypeDef

```python
# RunListItemTypeDef definition

class RunListItemTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    status: NotRequired[RunStatusType],  # (1)
    workflowId: NotRequired[str],
    name: NotRequired[str],
    priority: NotRequired[int],
    storageCapacity: NotRequired[int],
    creationTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
    stopTime: NotRequired[datetime],
    storageType: NotRequired[StorageTypeType],  # (2)
```

1. See [:material-code-brackets: RunStatusType](./literals.md#runstatustype) 
2. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListVariantImportJobsFilterTypeDef

```python
# ListVariantImportJobsFilterTypeDef definition

class ListVariantImportJobsFilterTypeDef(TypedDict):
    status: NotRequired[JobStatusType],  # (1)
    storeName: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## VariantImportJobItemTypeDef

```python
# VariantImportJobItemTypeDef definition

class VariantImportJobItemTypeDef(TypedDict):
    id: str,
    destinationName: str,
    roleArn: str,
    status: JobStatusType,  # (1)
    creationTime: datetime,
    updateTime: datetime,
    completionTime: NotRequired[datetime],
    runLeftNormalization: NotRequired[bool],
    annotationFields: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListVariantStoresFilterTypeDef

```python
# ListVariantStoresFilterTypeDef definition

class ListVariantStoresFilterTypeDef(TypedDict):
    status: NotRequired[StoreStatusType],  # (1)
```

1. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
## ListWorkflowsRequestRequestTypeDef

```python
# ListWorkflowsRequestRequestTypeDef definition

class ListWorkflowsRequestRequestTypeDef(TypedDict):
    type: NotRequired[WorkflowTypeType],  # (1)
    name: NotRequired[str],
    startingToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
## WorkflowListItemTypeDef

```python
# WorkflowListItemTypeDef definition

class WorkflowListItemTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[WorkflowStatusType],  # (1)
    type: NotRequired[WorkflowTypeType],  # (2)
    digest: NotRequired[str],
    creationTime: NotRequired[datetime],
    metadata: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: WorkflowStatusType](./literals.md#workflowstatustype) 
2. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
## PutS3AccessPolicyRequestRequestTypeDef

```python
# PutS3AccessPolicyRequestRequestTypeDef definition

class PutS3AccessPolicyRequestRequestTypeDef(TypedDict):
    s3AccessPointArn: str,
    s3AccessPolicy: str,
```

## ReadOptionsTypeDef

```python
# ReadOptionsTypeDef definition

class ReadOptionsTypeDef(TypedDict):
    sep: NotRequired[str],
    encoding: NotRequired[str],
    quote: NotRequired[str],
    quoteAll: NotRequired[bool],
    escape: NotRequired[str],
    escapeQuotes: NotRequired[bool],
    comment: NotRequired[str],
    header: NotRequired[bool],
    lineSep: NotRequired[str],
```

## StartReadSetActivationJobSourceItemTypeDef

```python
# StartReadSetActivationJobSourceItemTypeDef definition

class StartReadSetActivationJobSourceItemTypeDef(TypedDict):
    readSetId: str,
```

## StartReferenceImportJobSourceItemTypeDef

```python
# StartReferenceImportJobSourceItemTypeDef definition

class StartReferenceImportJobSourceItemTypeDef(TypedDict):
    sourceFile: str,
    name: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## StartRunRequestRequestTypeDef

```python
# StartRunRequestRequestTypeDef definition

class StartRunRequestRequestTypeDef(TypedDict):
    roleArn: str,
    requestId: str,
    workflowId: NotRequired[str],
    workflowType: NotRequired[WorkflowTypeType],  # (1)
    runId: NotRequired[str],
    name: NotRequired[str],
    cacheId: NotRequired[str],
    cacheBehavior: NotRequired[CacheBehaviorType],  # (2)
    runGroupId: NotRequired[str],
    priority: NotRequired[int],
    parameters: NotRequired[Mapping[str, Any]],
    storageCapacity: NotRequired[int],
    outputUri: NotRequired[str],
    logLevel: NotRequired[RunLogLevelType],  # (3)
    tags: NotRequired[Mapping[str, str]],
    retentionMode: NotRequired[RunRetentionModeType],  # (4)
    storageType: NotRequired[StorageTypeType],  # (5)
    workflowOwnerId: NotRequired[str],
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: CacheBehaviorType](./literals.md#cachebehaviortype) 
3. See [:material-code-brackets: RunLogLevelType](./literals.md#runlogleveltype) 
4. See [:material-code-brackets: RunRetentionModeType](./literals.md#runretentionmodetype) 
5. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
## VariantImportItemSourceTypeDef

```python
# VariantImportItemSourceTypeDef definition

class VariantImportItemSourceTypeDef(TypedDict):
    source: str,
```

## TsvStoreOptionsOutputTypeDef

```python
# TsvStoreOptionsOutputTypeDef definition

class TsvStoreOptionsOutputTypeDef(TypedDict):
    annotationType: NotRequired[AnnotationTypeType],  # (1)
    formatToHeader: NotRequired[Dict[FormatToHeaderKeyType, str]],  # (2)
    schema: NotRequired[List[Dict[str, SchemaValueTypeType]]],  # (3)
```

1. See [:material-code-brackets: AnnotationTypeType](./literals.md#annotationtypetype) 
2. See [:material-code-brackets: FormatToHeaderKeyType](./literals.md#formattoheaderkeytype) 
3. See [:material-code-brackets: SchemaValueTypeType](./literals.md#schemavaluetypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TsvStoreOptionsTypeDef

```python
# TsvStoreOptionsTypeDef definition

class TsvStoreOptionsTypeDef(TypedDict):
    annotationType: NotRequired[AnnotationTypeType],  # (1)
    formatToHeader: NotRequired[Mapping[FormatToHeaderKeyType, str]],  # (2)
    schema: NotRequired[Sequence[Mapping[str, SchemaValueTypeType]]],  # (3)
```

1. See [:material-code-brackets: AnnotationTypeType](./literals.md#annotationtypetype) 
2. See [:material-code-brackets: FormatToHeaderKeyType](./literals.md#formattoheaderkeytype) 
3. See [:material-code-brackets: SchemaValueTypeType](./literals.md#schemavaluetypetype) 
## TsvVersionOptionsOutputTypeDef

```python
# TsvVersionOptionsOutputTypeDef definition

class TsvVersionOptionsOutputTypeDef(TypedDict):
    annotationType: NotRequired[AnnotationTypeType],  # (1)
    formatToHeader: NotRequired[Dict[FormatToHeaderKeyType, str]],  # (2)
    schema: NotRequired[List[Dict[str, SchemaValueTypeType]]],  # (3)
```

1. See [:material-code-brackets: AnnotationTypeType](./literals.md#annotationtypetype) 
2. See [:material-code-brackets: FormatToHeaderKeyType](./literals.md#formattoheaderkeytype) 
3. See [:material-code-brackets: SchemaValueTypeType](./literals.md#schemavaluetypetype) 
## TsvVersionOptionsTypeDef

```python
# TsvVersionOptionsTypeDef definition

class TsvVersionOptionsTypeDef(TypedDict):
    annotationType: NotRequired[AnnotationTypeType],  # (1)
    formatToHeader: NotRequired[Mapping[FormatToHeaderKeyType, str]],  # (2)
    schema: NotRequired[Sequence[Mapping[str, SchemaValueTypeType]]],  # (3)
```

1. See [:material-code-brackets: AnnotationTypeType](./literals.md#annotationtypetype) 
2. See [:material-code-brackets: FormatToHeaderKeyType](./literals.md#formattoheaderkeytype) 
3. See [:material-code-brackets: SchemaValueTypeType](./literals.md#schemavaluetypetype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAnnotationStoreRequestRequestTypeDef

```python
# UpdateAnnotationStoreRequestRequestTypeDef definition

class UpdateAnnotationStoreRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
```

## UpdateAnnotationStoreVersionRequestRequestTypeDef

```python
# UpdateAnnotationStoreVersionRequestRequestTypeDef definition

class UpdateAnnotationStoreVersionRequestRequestTypeDef(TypedDict):
    name: str,
    versionName: str,
    description: NotRequired[str],
```

## UpdateRunCacheRequestRequestTypeDef

```python
# UpdateRunCacheRequestRequestTypeDef definition

class UpdateRunCacheRequestRequestTypeDef(TypedDict):
    id: str,
    cacheBehavior: NotRequired[CacheBehaviorType],  # (1)
    description: NotRequired[str],
    name: NotRequired[str],
```

1. See [:material-code-brackets: CacheBehaviorType](./literals.md#cachebehaviortype) 
## UpdateRunGroupRequestRequestTypeDef

```python
# UpdateRunGroupRequestRequestTypeDef definition

class UpdateRunGroupRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    maxCpus: NotRequired[int],
    maxRuns: NotRequired[int],
    maxDuration: NotRequired[int],
    maxGpus: NotRequired[int],
```

## UpdateVariantStoreRequestRequestTypeDef

```python
# UpdateVariantStoreRequestRequestTypeDef definition

class UpdateVariantStoreRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
```

## UpdateWorkflowRequestRequestTypeDef

```python
# UpdateWorkflowRequestRequestTypeDef definition

class UpdateWorkflowRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## AcceptShareResponseTypeDef

```python
# AcceptShareResponseTypeDef definition

class AcceptShareResponseTypeDef(TypedDict):
    status: ShareStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompleteMultipartReadSetUploadResponseTypeDef

```python
# CompleteMultipartReadSetUploadResponseTypeDef definition

class CompleteMultipartReadSetUploadResponseTypeDef(TypedDict):
    readSetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultipartReadSetUploadResponseTypeDef

```python
# CreateMultipartReadSetUploadResponseTypeDef definition

class CreateMultipartReadSetUploadResponseTypeDef(TypedDict):
    sequenceStoreId: str,
    uploadId: str,
    sourceFileType: FileTypeType,  # (1)
    subjectId: str,
    sampleId: str,
    generatedFrom: str,
    referenceArn: str,
    name: str,
    description: str,
    tags: Dict[str, str],
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRunCacheResponseTypeDef

```python
# CreateRunCacheResponseTypeDef definition

class CreateRunCacheResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: RunCacheStatusType,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RunCacheStatusType](./literals.md#runcachestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRunGroupResponseTypeDef

```python
# CreateRunGroupResponseTypeDef definition

class CreateRunGroupResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateShareResponseTypeDef

```python
# CreateShareResponseTypeDef definition

class CreateShareResponseTypeDef(TypedDict):
    shareId: str,
    status: ShareStatusType,  # (1)
    shareName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkflowResponseTypeDef

```python
# CreateWorkflowResponseTypeDef definition

class CreateWorkflowResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: WorkflowStatusType,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WorkflowStatusType](./literals.md#workflowstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAnnotationStoreResponseTypeDef

```python
# DeleteAnnotationStoreResponseTypeDef definition

class DeleteAnnotationStoreResponseTypeDef(TypedDict):
    status: StoreStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteShareResponseTypeDef

```python
# DeleteShareResponseTypeDef definition

class DeleteShareResponseTypeDef(TypedDict):
    status: ShareStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVariantStoreResponseTypeDef

```python
# DeleteVariantStoreResponseTypeDef definition

class DeleteVariantStoreResponseTypeDef(TypedDict):
    status: StoreStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReadSetResponseTypeDef

```python
# GetReadSetResponseTypeDef definition

class GetReadSetResponseTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReferenceResponseTypeDef

```python
# GetReferenceResponseTypeDef definition

class GetReferenceResponseTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRunCacheResponseTypeDef

```python
# GetRunCacheResponseTypeDef definition

class GetRunCacheResponseTypeDef(TypedDict):
    arn: str,
    cacheBehavior: CacheBehaviorType,  # (1)
    cacheBucketOwnerId: str,
    cacheS3Uri: str,
    creationTime: datetime,
    description: str,
    id: str,
    name: str,
    status: RunCacheStatusType,  # (2)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: CacheBehaviorType](./literals.md#cachebehaviortype) 
2. See [:material-code-brackets: RunCacheStatusType](./literals.md#runcachestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRunGroupResponseTypeDef

```python
# GetRunGroupResponseTypeDef definition

class GetRunGroupResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    maxCpus: int,
    maxRuns: int,
    maxDuration: int,
    creationTime: datetime,
    tags: Dict[str, str],
    maxGpus: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRunTaskResponseTypeDef

```python
# GetRunTaskResponseTypeDef definition

class GetRunTaskResponseTypeDef(TypedDict):
    taskId: str,
    status: TaskStatusType,  # (1)
    name: str,
    cpus: int,
    cacheHit: bool,
    cacheS3Uri: str,
    memory: int,
    creationTime: datetime,
    startTime: datetime,
    stopTime: datetime,
    statusMessage: str,
    logStream: str,
    gpus: int,
    instanceType: str,
    failureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetS3AccessPolicyResponseTypeDef

```python
# GetS3AccessPolicyResponseTypeDef definition

class GetS3AccessPolicyResponseTypeDef(TypedDict):
    s3AccessPointArn: str,
    storeId: str,
    storeType: StoreTypeType,  # (1)
    updateTime: datetime,
    s3AccessPolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StoreTypeType](./literals.md#storetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutS3AccessPolicyResponseTypeDef

```python
# PutS3AccessPolicyResponseTypeDef definition

class PutS3AccessPolicyResponseTypeDef(TypedDict):
    s3AccessPointArn: str,
    storeId: str,
    storeType: StoreTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StoreTypeType](./literals.md#storetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAnnotationImportResponseTypeDef

```python
# StartAnnotationImportResponseTypeDef definition

class StartAnnotationImportResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReadSetActivationJobResponseTypeDef

```python
# StartReadSetActivationJobResponseTypeDef definition

class StartReadSetActivationJobResponseTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    status: ReadSetActivationJobStatusType,  # (1)
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReadSetActivationJobStatusType](./literals.md#readsetactivationjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReadSetExportJobResponseTypeDef

```python
# StartReadSetExportJobResponseTypeDef definition

class StartReadSetExportJobResponseTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    destination: str,
    status: ReadSetExportJobStatusType,  # (1)
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReadSetExportJobStatusType](./literals.md#readsetexportjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReadSetImportJobResponseTypeDef

```python
# StartReadSetImportJobResponseTypeDef definition

class StartReadSetImportJobResponseTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    roleArn: str,
    status: ReadSetImportJobStatusType,  # (1)
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReadSetImportJobStatusType](./literals.md#readsetimportjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReferenceImportJobResponseTypeDef

```python
# StartReferenceImportJobResponseTypeDef definition

class StartReferenceImportJobResponseTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
    roleArn: str,
    status: ReferenceImportJobStatusType,  # (1)
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReferenceImportJobStatusType](./literals.md#referenceimportjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRunResponseTypeDef

```python
# StartRunResponseTypeDef definition

class StartRunResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: RunStatusType,  # (1)
    tags: Dict[str, str],
    uuid: str,
    runOutputUri: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RunStatusType](./literals.md#runstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartVariantImportResponseTypeDef

```python
# StartVariantImportResponseTypeDef definition

class StartVariantImportResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnnotationStoreVersionResponseTypeDef

```python
# UpdateAnnotationStoreVersionResponseTypeDef definition

class UpdateAnnotationStoreVersionResponseTypeDef(TypedDict):
    storeId: str,
    id: str,
    status: VersionStatusType,  # (1)
    name: str,
    versionName: str,
    description: str,
    creationTime: datetime,
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadReadSetPartResponseTypeDef

```python
# UploadReadSetPartResponseTypeDef definition

class UploadReadSetPartResponseTypeDef(TypedDict):
    checksum: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivateReadSetFilterTypeDef

```python
# ActivateReadSetFilterTypeDef definition

class ActivateReadSetFilterTypeDef(TypedDict):
    status: NotRequired[ReadSetActivationJobStatusType],  # (1)
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ReadSetActivationJobStatusType](./literals.md#readsetactivationjobstatustype) 
## ExportReadSetFilterTypeDef

```python
# ExportReadSetFilterTypeDef definition

class ExportReadSetFilterTypeDef(TypedDict):
    status: NotRequired[ReadSetExportJobStatusType],  # (1)
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ReadSetExportJobStatusType](./literals.md#readsetexportjobstatustype) 
## ImportReadSetFilterTypeDef

```python
# ImportReadSetFilterTypeDef definition

class ImportReadSetFilterTypeDef(TypedDict):
    status: NotRequired[ReadSetImportJobStatusType],  # (1)
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ReadSetImportJobStatusType](./literals.md#readsetimportjobstatustype) 
## ImportReferenceFilterTypeDef

```python
# ImportReferenceFilterTypeDef definition

class ImportReferenceFilterTypeDef(TypedDict):
    status: NotRequired[ReferenceImportJobStatusType],  # (1)
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ReferenceImportJobStatusType](./literals.md#referenceimportjobstatustype) 
## ReadSetFilterTypeDef

```python
# ReadSetFilterTypeDef definition

class ReadSetFilterTypeDef(TypedDict):
    name: NotRequired[str],
    status: NotRequired[ReadSetStatusType],  # (1)
    referenceArn: NotRequired[str],
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
    sampleId: NotRequired[str],
    subjectId: NotRequired[str],
    generatedFrom: NotRequired[str],
    creationType: NotRequired[CreationTypeType],  # (2)
```

1. See [:material-code-brackets: ReadSetStatusType](./literals.md#readsetstatustype) 
2. See [:material-code-brackets: CreationTypeType](./literals.md#creationtypetype) 
## ReadSetUploadPartListFilterTypeDef

```python
# ReadSetUploadPartListFilterTypeDef definition

class ReadSetUploadPartListFilterTypeDef(TypedDict):
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
```

## ReferenceFilterTypeDef

```python
# ReferenceFilterTypeDef definition

class ReferenceFilterTypeDef(TypedDict):
    name: NotRequired[str],
    md5: NotRequired[str],
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
```

## ReferenceStoreFilterTypeDef

```python
# ReferenceStoreFilterTypeDef definition

class ReferenceStoreFilterTypeDef(TypedDict):
    name: NotRequired[str],
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
```

## SequenceStoreFilterTypeDef

```python
# SequenceStoreFilterTypeDef definition

class SequenceStoreFilterTypeDef(TypedDict):
    name: NotRequired[str],
    createdAfter: NotRequired[TimestampTypeDef],
    createdBefore: NotRequired[TimestampTypeDef],
    status: NotRequired[SequenceStoreStatusType],  # (1)
    updatedAfter: NotRequired[TimestampTypeDef],
    updatedBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: SequenceStoreStatusType](./literals.md#sequencestorestatustype) 
## ListReadSetActivationJobsResponseTypeDef

```python
# ListReadSetActivationJobsResponseTypeDef definition

class ListReadSetActivationJobsResponseTypeDef(TypedDict):
    activationJobs: List[ActivateReadSetJobItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ActivateReadSetJobItemTypeDef](./type_defs.md#activatereadsetjobitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReadSetActivationJobResponseTypeDef

```python
# GetReadSetActivationJobResponseTypeDef definition

class GetReadSetActivationJobResponseTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    status: ReadSetActivationJobStatusType,  # (1)
    statusMessage: str,
    creationTime: datetime,
    completionTime: datetime,
    sources: List[ActivateReadSetSourceItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ReadSetActivationJobStatusType](./literals.md#readsetactivationjobstatustype) 
2. See [:material-code-braces: ActivateReadSetSourceItemTypeDef](./type_defs.md#activatereadsetsourceitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnnotationImportJobsResponseTypeDef

```python
# ListAnnotationImportJobsResponseTypeDef definition

class ListAnnotationImportJobsResponseTypeDef(TypedDict):
    annotationImportJobs: List[AnnotationImportJobItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnnotationImportJobItemTypeDef](./type_defs.md#annotationimportjobitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVariantStoreResponseTypeDef

```python
# CreateVariantStoreResponseTypeDef definition

class CreateVariantStoreResponseTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    status: StoreStatusType,  # (2)
    name: str,
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVariantStoreResponseTypeDef

```python
# UpdateVariantStoreResponseTypeDef definition

class UpdateVariantStoreResponseTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    status: StoreStatusType,  # (2)
    name: str,
    description: str,
    creationTime: datetime,
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnnotationStoreItemTypeDef

```python
# AnnotationStoreItemTypeDef definition

class AnnotationStoreItemTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    status: StoreStatusType,  # (2)
    storeArn: str,
    name: str,
    storeFormat: StoreFormatType,  # (3)
    description: str,
    sseConfig: SseConfigTypeDef,  # (4)
    creationTime: datetime,
    updateTime: datetime,
    statusMessage: str,
    storeSizeBytes: int,
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
3. See [:material-code-brackets: StoreFormatType](./literals.md#storeformattype) 
4. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
## CreateReferenceStoreRequestRequestTypeDef

```python
# CreateReferenceStoreRequestRequestTypeDef definition

class CreateReferenceStoreRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    sseConfig: NotRequired[SseConfigTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
## CreateReferenceStoreResponseTypeDef

```python
# CreateReferenceStoreResponseTypeDef definition

class CreateReferenceStoreResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (1)
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVariantStoreRequestRequestTypeDef

```python
# CreateVariantStoreRequestRequestTypeDef definition

class CreateVariantStoreRequestRequestTypeDef(TypedDict):
    reference: ReferenceItemTypeDef,  # (1)
    name: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    sseConfig: NotRequired[SseConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
## GetReferenceStoreResponseTypeDef

```python
# GetReferenceStoreResponseTypeDef definition

class GetReferenceStoreResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (1)
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVariantStoreResponseTypeDef

```python
# GetVariantStoreResponseTypeDef definition

class GetVariantStoreResponseTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    status: StoreStatusType,  # (2)
    storeArn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (3)
    creationTime: datetime,
    updateTime: datetime,
    tags: Dict[str, str],
    statusMessage: str,
    storeSizeBytes: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
3. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReferenceStoreDetailTypeDef

```python
# ReferenceStoreDetailTypeDef definition

class ReferenceStoreDetailTypeDef(TypedDict):
    arn: str,
    id: str,
    creationTime: datetime,
    name: NotRequired[str],
    description: NotRequired[str],
    sseConfig: NotRequired[SseConfigTypeDef],  # (1)
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
## SequenceStoreDetailTypeDef

```python
# SequenceStoreDetailTypeDef definition

class SequenceStoreDetailTypeDef(TypedDict):
    arn: str,
    id: str,
    creationTime: datetime,
    name: NotRequired[str],
    description: NotRequired[str],
    sseConfig: NotRequired[SseConfigTypeDef],  # (1)
    fallbackLocation: NotRequired[str],
    eTagAlgorithmFamily: NotRequired[ETagAlgorithmFamilyType],  # (2)
    status: NotRequired[SequenceStoreStatusType],  # (3)
    statusMessage: NotRequired[str],
    updateTime: NotRequired[datetime],
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-brackets: ETagAlgorithmFamilyType](./literals.md#etagalgorithmfamilytype) 
3. See [:material-code-brackets: SequenceStoreStatusType](./literals.md#sequencestorestatustype) 
## VariantStoreItemTypeDef

```python
# VariantStoreItemTypeDef definition

class VariantStoreItemTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    status: StoreStatusType,  # (2)
    storeArn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (3)
    creationTime: datetime,
    updateTime: datetime,
    statusMessage: str,
    storeSizeBytes: int,
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
3. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
## ListAnnotationStoreVersionsResponseTypeDef

```python
# ListAnnotationStoreVersionsResponseTypeDef definition

class ListAnnotationStoreVersionsResponseTypeDef(TypedDict):
    annotationStoreVersions: List[AnnotationStoreVersionItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnnotationStoreVersionItemTypeDef](./type_defs.md#annotationstoreversionitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteReadSetResponseTypeDef

```python
# BatchDeleteReadSetResponseTypeDef definition

class BatchDeleteReadSetResponseTypeDef(TypedDict):
    errors: List[ReadSetBatchErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReadSetBatchErrorTypeDef](./type_defs.md#readsetbatcherrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadReadSetPartRequestRequestTypeDef

```python
# UploadReadSetPartRequestRequestTypeDef definition

class UploadReadSetPartRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    uploadId: str,
    partSource: ReadSetPartSourceType,  # (1)
    partNumber: int,
    payload: BlobTypeDef,
```

1. See [:material-code-brackets: ReadSetPartSourceType](./literals.md#readsetpartsourcetype) 
## CompleteMultipartReadSetUploadRequestRequestTypeDef

```python
# CompleteMultipartReadSetUploadRequestRequestTypeDef definition

class CompleteMultipartReadSetUploadRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    uploadId: str,
    parts: Sequence[CompleteReadSetUploadPartListItemTypeDef],  # (1)
```

1. See [:material-code-braces: CompleteReadSetUploadPartListItemTypeDef](./type_defs.md#completereadsetuploadpartlistitemtypedef) 
## CreateSequenceStoreRequestRequestTypeDef

```python
# CreateSequenceStoreRequestRequestTypeDef definition

class CreateSequenceStoreRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    sseConfig: NotRequired[SseConfigTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    fallbackLocation: NotRequired[str],
    eTagAlgorithmFamily: NotRequired[ETagAlgorithmFamilyType],  # (2)
    propagatedSetLevelTags: NotRequired[Sequence[str]],
    s3AccessConfig: NotRequired[S3AccessConfigTypeDef],  # (3)
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-brackets: ETagAlgorithmFamilyType](./literals.md#etagalgorithmfamilytype) 
3. See [:material-code-braces: S3AccessConfigTypeDef](./type_defs.md#s3accessconfigtypedef) 
## UpdateSequenceStoreRequestRequestTypeDef

```python
# UpdateSequenceStoreRequestRequestTypeDef definition

class UpdateSequenceStoreRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    description: NotRequired[str],
    clientToken: NotRequired[str],
    fallbackLocation: NotRequired[str],
    propagatedSetLevelTags: NotRequired[Sequence[str]],
    s3AccessConfig: NotRequired[S3AccessConfigTypeDef],  # (1)
```

1. See [:material-code-braces: S3AccessConfigTypeDef](./type_defs.md#s3accessconfigtypedef) 
## CreateSequenceStoreResponseTypeDef

```python
# CreateSequenceStoreResponseTypeDef definition

class CreateSequenceStoreResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (1)
    creationTime: datetime,
    fallbackLocation: str,
    eTagAlgorithmFamily: ETagAlgorithmFamilyType,  # (2)
    status: SequenceStoreStatusType,  # (3)
    statusMessage: str,
    propagatedSetLevelTags: List[str],
    s3Access: SequenceStoreS3AccessTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-brackets: ETagAlgorithmFamilyType](./literals.md#etagalgorithmfamilytype) 
3. See [:material-code-brackets: SequenceStoreStatusType](./literals.md#sequencestorestatustype) 
4. See [:material-code-braces: SequenceStoreS3AccessTypeDef](./type_defs.md#sequencestores3accesstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSequenceStoreResponseTypeDef

```python
# GetSequenceStoreResponseTypeDef definition

class GetSequenceStoreResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (1)
    creationTime: datetime,
    fallbackLocation: str,
    s3Access: SequenceStoreS3AccessTypeDef,  # (2)
    eTagAlgorithmFamily: ETagAlgorithmFamilyType,  # (3)
    status: SequenceStoreStatusType,  # (4)
    statusMessage: str,
    propagatedSetLevelTags: List[str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-braces: SequenceStoreS3AccessTypeDef](./type_defs.md#sequencestores3accesstypedef) 
3. See [:material-code-brackets: ETagAlgorithmFamilyType](./literals.md#etagalgorithmfamilytype) 
4. See [:material-code-brackets: SequenceStoreStatusType](./literals.md#sequencestorestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSequenceStoreResponseTypeDef

```python
# UpdateSequenceStoreResponseTypeDef definition

class UpdateSequenceStoreResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (1)
    creationTime: datetime,
    updateTime: datetime,
    propagatedSetLevelTags: List[str],
    status: SequenceStoreStatusType,  # (2)
    statusMessage: str,
    fallbackLocation: str,
    s3Access: SequenceStoreS3AccessTypeDef,  # (3)
    eTagAlgorithmFamily: ETagAlgorithmFamilyType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
2. See [:material-code-brackets: SequenceStoreStatusType](./literals.md#sequencestorestatustype) 
3. See [:material-code-braces: SequenceStoreS3AccessTypeDef](./type_defs.md#sequencestores3accesstypedef) 
4. See [:material-code-brackets: ETagAlgorithmFamilyType](./literals.md#etagalgorithmfamilytype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkflowRequestRequestTypeDef

```python
# CreateWorkflowRequestRequestTypeDef definition

class CreateWorkflowRequestRequestTypeDef(TypedDict):
    requestId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    engine: NotRequired[WorkflowEngineType],  # (1)
    definitionZip: NotRequired[BlobTypeDef],
    definitionUri: NotRequired[str],
    main: NotRequired[str],
    parameterTemplate: NotRequired[Mapping[str, WorkflowParameterTypeDef]],  # (2)
    storageCapacity: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
    accelerators: NotRequired[AcceleratorsType],  # (3)
```

1. See [:material-code-brackets: WorkflowEngineType](./literals.md#workflowenginetype) 
2. See [:material-code-braces: WorkflowParameterTypeDef](./type_defs.md#workflowparametertypedef) 
3. See [:material-code-brackets: AcceleratorsType](./literals.md#acceleratorstype) 
## GetWorkflowResponseTypeDef

```python
# GetWorkflowResponseTypeDef definition

class GetWorkflowResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    status: WorkflowStatusType,  # (1)
    type: WorkflowTypeType,  # (2)
    name: str,
    description: str,
    engine: WorkflowEngineType,  # (3)
    definition: str,
    main: str,
    digest: str,
    parameterTemplate: Dict[str, WorkflowParameterTypeDef],  # (4)
    storageCapacity: int,
    creationTime: datetime,
    statusMessage: str,
    tags: Dict[str, str],
    metadata: Dict[str, str],
    accelerators: AcceleratorsType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: WorkflowStatusType](./literals.md#workflowstatustype) 
2. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
3. See [:material-code-brackets: WorkflowEngineType](./literals.md#workflowenginetype) 
4. See [:material-code-braces: WorkflowParameterTypeDef](./type_defs.md#workflowparametertypedef) 
5. See [:material-code-brackets: AcceleratorsType](./literals.md#acceleratorstype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAnnotationStoreVersionsResponseTypeDef

```python
# DeleteAnnotationStoreVersionsResponseTypeDef definition

class DeleteAnnotationStoreVersionsResponseTypeDef(TypedDict):
    errors: List[VersionDeleteErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VersionDeleteErrorTypeDef](./type_defs.md#versiondeleteerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReadSetExportJobResponseTypeDef

```python
# GetReadSetExportJobResponseTypeDef definition

class GetReadSetExportJobResponseTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    destination: str,
    status: ReadSetExportJobStatusType,  # (1)
    statusMessage: str,
    creationTime: datetime,
    completionTime: datetime,
    readSets: List[ExportReadSetDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ReadSetExportJobStatusType](./literals.md#readsetexportjobstatustype) 
2. See [:material-code-braces: ExportReadSetDetailTypeDef](./type_defs.md#exportreadsetdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReadSetExportJobsResponseTypeDef

```python
# ListReadSetExportJobsResponseTypeDef definition

class ListReadSetExportJobsResponseTypeDef(TypedDict):
    exportJobs: List[ExportReadSetJobDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportReadSetJobDetailTypeDef](./type_defs.md#exportreadsetjobdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReadSetExportJobRequestRequestTypeDef

```python
# StartReadSetExportJobRequestRequestTypeDef definition

class StartReadSetExportJobRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    destination: str,
    roleArn: str,
    sources: Sequence[ExportReadSetTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: ExportReadSetTypeDef](./type_defs.md#exportreadsettypedef) 
## FileInformationTypeDef

```python
# FileInformationTypeDef definition

class FileInformationTypeDef(TypedDict):
    totalParts: NotRequired[int],
    partSize: NotRequired[int],
    contentLength: NotRequired[int],
    s3Access: NotRequired[ReadSetS3AccessTypeDef],  # (1)
```

1. See [:material-code-braces: ReadSetS3AccessTypeDef](./type_defs.md#readsets3accesstypedef) 
## ListSharesRequestRequestTypeDef

```python
# ListSharesRequestRequestTypeDef definition

class ListSharesRequestRequestTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    filter: NotRequired[FilterTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetAnnotationImportRequestWaitTypeDef

```python
# GetAnnotationImportRequestWaitTypeDef definition

class GetAnnotationImportRequestWaitTypeDef(TypedDict):
    jobId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetAnnotationStoreRequestWaitTypeDef

```python
# GetAnnotationStoreRequestWaitTypeDef definition

class GetAnnotationStoreRequestWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetAnnotationStoreVersionRequestWaitTypeDef

```python
# GetAnnotationStoreVersionRequestWaitTypeDef definition

class GetAnnotationStoreVersionRequestWaitTypeDef(TypedDict):
    name: str,
    versionName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetReadSetActivationJobRequestWaitTypeDef

```python
# GetReadSetActivationJobRequestWaitTypeDef definition

class GetReadSetActivationJobRequestWaitTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetReadSetExportJobRequestWaitTypeDef

```python
# GetReadSetExportJobRequestWaitTypeDef definition

class GetReadSetExportJobRequestWaitTypeDef(TypedDict):
    sequenceStoreId: str,
    id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetReadSetImportJobRequestWaitTypeDef

```python
# GetReadSetImportJobRequestWaitTypeDef definition

class GetReadSetImportJobRequestWaitTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetReferenceImportJobRequestWaitTypeDef

```python
# GetReferenceImportJobRequestWaitTypeDef definition

class GetReferenceImportJobRequestWaitTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetRunRequestWaitTypeDef

```python
# GetRunRequestWaitTypeDef definition

class GetRunRequestWaitTypeDef(TypedDict):
    id: str,
    export: NotRequired[Sequence[RunExportType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RunExportType](./literals.md#runexporttype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetRunTaskRequestWaitTypeDef

```python
# GetRunTaskRequestWaitTypeDef definition

class GetRunTaskRequestWaitTypeDef(TypedDict):
    id: str,
    taskId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetVariantImportRequestWaitTypeDef

```python
# GetVariantImportRequestWaitTypeDef definition

class GetVariantImportRequestWaitTypeDef(TypedDict):
    jobId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetVariantStoreRequestWaitTypeDef

```python
# GetVariantStoreRequestWaitTypeDef definition

class GetVariantStoreRequestWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetWorkflowRequestWaitTypeDef

```python
# GetWorkflowRequestWaitTypeDef definition

class GetWorkflowRequestWaitTypeDef(TypedDict):
    id: str,
    type: NotRequired[WorkflowTypeType],  # (1)
    export: NotRequired[Sequence[WorkflowExportType]],  # (2)
    workflowOwnerId: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: WorkflowExportType](./literals.md#workflowexporttype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ReadSetListItemTypeDef

```python
# ReadSetListItemTypeDef definition

class ReadSetListItemTypeDef(TypedDict):
    id: str,
    arn: str,
    sequenceStoreId: str,
    status: ReadSetStatusType,  # (1)
    fileType: FileTypeType,  # (2)
    creationTime: datetime,
    subjectId: NotRequired[str],
    sampleId: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    referenceArn: NotRequired[str],
    sequenceInformation: NotRequired[SequenceInformationTypeDef],  # (3)
    statusMessage: NotRequired[str],
    creationType: NotRequired[CreationTypeType],  # (4)
    etag: NotRequired[ETagTypeDef],  # (5)
```

1. See [:material-code-brackets: ReadSetStatusType](./literals.md#readsetstatustype) 
2. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
3. See [:material-code-braces: SequenceInformationTypeDef](./type_defs.md#sequenceinformationtypedef) 
4. See [:material-code-brackets: CreationTypeType](./literals.md#creationtypetype) 
5. See [:material-code-braces: ETagTypeDef](./type_defs.md#etagtypedef) 
## GetReferenceImportJobResponseTypeDef

```python
# GetReferenceImportJobResponseTypeDef definition

class GetReferenceImportJobResponseTypeDef(TypedDict):
    id: str,
    referenceStoreId: str,
    roleArn: str,
    status: ReferenceImportJobStatusType,  # (1)
    statusMessage: str,
    creationTime: datetime,
    completionTime: datetime,
    sources: List[ImportReferenceSourceItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ReferenceImportJobStatusType](./literals.md#referenceimportjobstatustype) 
2. See [:material-code-braces: ImportReferenceSourceItemTypeDef](./type_defs.md#importreferencesourceitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRunResponseTypeDef

```python
# GetRunResponseTypeDef definition

class GetRunResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    cacheId: str,
    cacheBehavior: CacheBehaviorType,  # (1)
    engineVersion: str,
    status: RunStatusType,  # (2)
    workflowId: str,
    workflowType: WorkflowTypeType,  # (3)
    runId: str,
    roleArn: str,
    name: str,
    runGroupId: str,
    priority: int,
    definition: str,
    digest: str,
    parameters: Dict[str, Any],
    storageCapacity: int,
    outputUri: str,
    logLevel: RunLogLevelType,  # (4)
    resourceDigests: Dict[str, str],
    startedBy: str,
    creationTime: datetime,
    startTime: datetime,
    stopTime: datetime,
    statusMessage: str,
    tags: Dict[str, str],
    accelerators: AcceleratorsType,  # (5)
    retentionMode: RunRetentionModeType,  # (6)
    failureReason: str,
    logLocation: RunLogLocationTypeDef,  # (7)
    uuid: str,
    runOutputUri: str,
    storageType: StorageTypeType,  # (8)
    workflowOwnerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: CacheBehaviorType](./literals.md#cachebehaviortype) 
2. See [:material-code-brackets: RunStatusType](./literals.md#runstatustype) 
3. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
4. See [:material-code-brackets: RunLogLevelType](./literals.md#runlogleveltype) 
5. See [:material-code-brackets: AcceleratorsType](./literals.md#acceleratorstype) 
6. See [:material-code-brackets: RunRetentionModeType](./literals.md#runretentionmodetype) 
7. See [:material-code-braces: RunLogLocationTypeDef](./type_defs.md#runloglocationtypedef) 
8. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetShareResponseTypeDef

```python
# GetShareResponseTypeDef definition

class GetShareResponseTypeDef(TypedDict):
    share: ShareDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ShareDetailsTypeDef](./type_defs.md#sharedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSharesResponseTypeDef

```python
# ListSharesResponseTypeDef definition

class ListSharesResponseTypeDef(TypedDict):
    shares: List[ShareDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ShareDetailsTypeDef](./type_defs.md#sharedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVariantImportResponseTypeDef

```python
# GetVariantImportResponseTypeDef definition

class GetVariantImportResponseTypeDef(TypedDict):
    id: str,
    destinationName: str,
    roleArn: str,
    status: JobStatusType,  # (1)
    statusMessage: str,
    creationTime: datetime,
    updateTime: datetime,
    completionTime: datetime,
    items: List[VariantImportItemDetailTypeDef],  # (2)
    runLeftNormalization: bool,
    annotationFields: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: VariantImportItemDetailTypeDef](./type_defs.md#variantimportitemdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReadSetImportJobsResponseTypeDef

```python
# ListReadSetImportJobsResponseTypeDef definition

class ListReadSetImportJobsResponseTypeDef(TypedDict):
    importJobs: List[ImportReadSetJobItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportReadSetJobItemTypeDef](./type_defs.md#importreadsetjobitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportReadSetSourceItemTypeDef

```python
# ImportReadSetSourceItemTypeDef definition

class ImportReadSetSourceItemTypeDef(TypedDict):
    sourceFiles: SourceFilesTypeDef,  # (1)
    sourceFileType: FileTypeType,  # (2)
    status: ReadSetImportJobItemStatusType,  # (3)
    subjectId: str,
    sampleId: str,
    statusMessage: NotRequired[str],
    generatedFrom: NotRequired[str],
    referenceArn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    readSetId: NotRequired[str],
```

1. See [:material-code-braces: SourceFilesTypeDef](./type_defs.md#sourcefilestypedef) 
2. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
3. See [:material-code-brackets: ReadSetImportJobItemStatusType](./literals.md#readsetimportjobitemstatustype) 
## StartReadSetImportJobSourceItemTypeDef

```python
# StartReadSetImportJobSourceItemTypeDef definition

class StartReadSetImportJobSourceItemTypeDef(TypedDict):
    sourceFiles: SourceFilesTypeDef,  # (1)
    sourceFileType: FileTypeType,  # (2)
    subjectId: str,
    sampleId: str,
    generatedFrom: NotRequired[str],
    referenceArn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SourceFilesTypeDef](./type_defs.md#sourcefilestypedef) 
2. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
## ListReferenceImportJobsResponseTypeDef

```python
# ListReferenceImportJobsResponseTypeDef definition

class ListReferenceImportJobsResponseTypeDef(TypedDict):
    importJobs: List[ImportReferenceJobItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportReferenceJobItemTypeDef](./type_defs.md#importreferencejobitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnnotationImportJobsRequestRequestTypeDef

```python
# ListAnnotationImportJobsRequestRequestTypeDef definition

class ListAnnotationImportJobsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    ids: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    filter: NotRequired[ListAnnotationImportJobsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListAnnotationImportJobsFilterTypeDef](./type_defs.md#listannotationimportjobsfiltertypedef) 
## ListAnnotationImportJobsRequestPaginateTypeDef

```python
# ListAnnotationImportJobsRequestPaginateTypeDef definition

class ListAnnotationImportJobsRequestPaginateTypeDef(TypedDict):
    ids: NotRequired[Sequence[str]],
    filter: NotRequired[ListAnnotationImportJobsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListAnnotationImportJobsFilterTypeDef](./type_defs.md#listannotationimportjobsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMultipartReadSetUploadsRequestPaginateTypeDef

```python
# ListMultipartReadSetUploadsRequestPaginateTypeDef definition

class ListMultipartReadSetUploadsRequestPaginateTypeDef(TypedDict):
    sequenceStoreId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRunCachesRequestPaginateTypeDef

```python
# ListRunCachesRequestPaginateTypeDef definition

class ListRunCachesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRunGroupsRequestPaginateTypeDef

```python
# ListRunGroupsRequestPaginateTypeDef definition

class ListRunGroupsRequestPaginateTypeDef(TypedDict):
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRunTasksRequestPaginateTypeDef

```python
# ListRunTasksRequestPaginateTypeDef definition

class ListRunTasksRequestPaginateTypeDef(TypedDict):
    id: str,
    status: NotRequired[TaskStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRunsRequestPaginateTypeDef

```python
# ListRunsRequestPaginateTypeDef definition

class ListRunsRequestPaginateTypeDef(TypedDict):
    name: NotRequired[str],
    runGroupId: NotRequired[str],
    status: NotRequired[RunStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RunStatusType](./literals.md#runstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSharesRequestPaginateTypeDef

```python
# ListSharesRequestPaginateTypeDef definition

class ListSharesRequestPaginateTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    filter: NotRequired[FilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkflowsRequestPaginateTypeDef

```python
# ListWorkflowsRequestPaginateTypeDef definition

class ListWorkflowsRequestPaginateTypeDef(TypedDict):
    type: NotRequired[WorkflowTypeType],  # (1)
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnnotationStoreVersionsRequestPaginateTypeDef

```python
# ListAnnotationStoreVersionsRequestPaginateTypeDef definition

class ListAnnotationStoreVersionsRequestPaginateTypeDef(TypedDict):
    name: str,
    filter: NotRequired[ListAnnotationStoreVersionsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListAnnotationStoreVersionsFilterTypeDef](./type_defs.md#listannotationstoreversionsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnnotationStoreVersionsRequestRequestTypeDef

```python
# ListAnnotationStoreVersionsRequestRequestTypeDef definition

class ListAnnotationStoreVersionsRequestRequestTypeDef(TypedDict):
    name: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ListAnnotationStoreVersionsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListAnnotationStoreVersionsFilterTypeDef](./type_defs.md#listannotationstoreversionsfiltertypedef) 
## ListAnnotationStoresRequestPaginateTypeDef

```python
# ListAnnotationStoresRequestPaginateTypeDef definition

class ListAnnotationStoresRequestPaginateTypeDef(TypedDict):
    ids: NotRequired[Sequence[str]],
    filter: NotRequired[ListAnnotationStoresFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListAnnotationStoresFilterTypeDef](./type_defs.md#listannotationstoresfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnnotationStoresRequestRequestTypeDef

```python
# ListAnnotationStoresRequestRequestTypeDef definition

class ListAnnotationStoresRequestRequestTypeDef(TypedDict):
    ids: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ListAnnotationStoresFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListAnnotationStoresFilterTypeDef](./type_defs.md#listannotationstoresfiltertypedef) 
## ListMultipartReadSetUploadsResponseTypeDef

```python
# ListMultipartReadSetUploadsResponseTypeDef definition

class ListMultipartReadSetUploadsResponseTypeDef(TypedDict):
    uploads: List[MultipartReadSetUploadListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MultipartReadSetUploadListItemTypeDef](./type_defs.md#multipartreadsetuploadlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReadSetUploadPartsResponseTypeDef

```python
# ListReadSetUploadPartsResponseTypeDef definition

class ListReadSetUploadPartsResponseTypeDef(TypedDict):
    parts: List[ReadSetUploadPartListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReadSetUploadPartListItemTypeDef](./type_defs.md#readsetuploadpartlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReferencesResponseTypeDef

```python
# ListReferencesResponseTypeDef definition

class ListReferencesResponseTypeDef(TypedDict):
    references: List[ReferenceListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReferenceListItemTypeDef](./type_defs.md#referencelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRunCachesResponseTypeDef

```python
# ListRunCachesResponseTypeDef definition

class ListRunCachesResponseTypeDef(TypedDict):
    items: List[RunCacheListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RunCacheListItemTypeDef](./type_defs.md#runcachelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRunGroupsResponseTypeDef

```python
# ListRunGroupsResponseTypeDef definition

class ListRunGroupsResponseTypeDef(TypedDict):
    items: List[RunGroupListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RunGroupListItemTypeDef](./type_defs.md#rungrouplistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRunTasksResponseTypeDef

```python
# ListRunTasksResponseTypeDef definition

class ListRunTasksResponseTypeDef(TypedDict):
    items: List[TaskListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TaskListItemTypeDef](./type_defs.md#tasklistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRunsResponseTypeDef

```python
# ListRunsResponseTypeDef definition

class ListRunsResponseTypeDef(TypedDict):
    items: List[RunListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RunListItemTypeDef](./type_defs.md#runlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVariantImportJobsRequestPaginateTypeDef

```python
# ListVariantImportJobsRequestPaginateTypeDef definition

class ListVariantImportJobsRequestPaginateTypeDef(TypedDict):
    ids: NotRequired[Sequence[str]],
    filter: NotRequired[ListVariantImportJobsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListVariantImportJobsFilterTypeDef](./type_defs.md#listvariantimportjobsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVariantImportJobsRequestRequestTypeDef

```python
# ListVariantImportJobsRequestRequestTypeDef definition

class ListVariantImportJobsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    ids: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    filter: NotRequired[ListVariantImportJobsFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListVariantImportJobsFilterTypeDef](./type_defs.md#listvariantimportjobsfiltertypedef) 
## ListVariantImportJobsResponseTypeDef

```python
# ListVariantImportJobsResponseTypeDef definition

class ListVariantImportJobsResponseTypeDef(TypedDict):
    variantImportJobs: List[VariantImportJobItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VariantImportJobItemTypeDef](./type_defs.md#variantimportjobitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVariantStoresRequestPaginateTypeDef

```python
# ListVariantStoresRequestPaginateTypeDef definition

class ListVariantStoresRequestPaginateTypeDef(TypedDict):
    ids: NotRequired[Sequence[str]],
    filter: NotRequired[ListVariantStoresFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListVariantStoresFilterTypeDef](./type_defs.md#listvariantstoresfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVariantStoresRequestRequestTypeDef

```python
# ListVariantStoresRequestRequestTypeDef definition

class ListVariantStoresRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    ids: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    filter: NotRequired[ListVariantStoresFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListVariantStoresFilterTypeDef](./type_defs.md#listvariantstoresfiltertypedef) 
## ListWorkflowsResponseTypeDef

```python
# ListWorkflowsResponseTypeDef definition

class ListWorkflowsResponseTypeDef(TypedDict):
    items: List[WorkflowListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkflowListItemTypeDef](./type_defs.md#workflowlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TsvOptionsTypeDef

```python
# TsvOptionsTypeDef definition

class TsvOptionsTypeDef(TypedDict):
    readOptions: NotRequired[ReadOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: ReadOptionsTypeDef](./type_defs.md#readoptionstypedef) 
## StartReadSetActivationJobRequestRequestTypeDef

```python
# StartReadSetActivationJobRequestRequestTypeDef definition

class StartReadSetActivationJobRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    sources: Sequence[StartReadSetActivationJobSourceItemTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: StartReadSetActivationJobSourceItemTypeDef](./type_defs.md#startreadsetactivationjobsourceitemtypedef) 
## StartReferenceImportJobRequestRequestTypeDef

```python
# StartReferenceImportJobRequestRequestTypeDef definition

class StartReferenceImportJobRequestRequestTypeDef(TypedDict):
    referenceStoreId: str,
    roleArn: str,
    sources: Sequence[StartReferenceImportJobSourceItemTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: StartReferenceImportJobSourceItemTypeDef](./type_defs.md#startreferenceimportjobsourceitemtypedef) 
## StartVariantImportRequestRequestTypeDef

```python
# StartVariantImportRequestRequestTypeDef definition

class StartVariantImportRequestRequestTypeDef(TypedDict):
    destinationName: str,
    roleArn: str,
    items: Sequence[VariantImportItemSourceTypeDef],  # (1)
    runLeftNormalization: NotRequired[bool],
    annotationFields: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: VariantImportItemSourceTypeDef](./type_defs.md#variantimportitemsourcetypedef) 
## StoreOptionsOutputTypeDef

```python
# StoreOptionsOutputTypeDef definition

class StoreOptionsOutputTypeDef(TypedDict):
    tsvStoreOptions: NotRequired[TsvStoreOptionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: TsvStoreOptionsOutputTypeDef](./type_defs.md#tsvstoreoptionsoutputtypedef) 
## VersionOptionsOutputTypeDef

```python
# VersionOptionsOutputTypeDef definition

class VersionOptionsOutputTypeDef(TypedDict):
    tsvVersionOptions: NotRequired[TsvVersionOptionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: TsvVersionOptionsOutputTypeDef](./type_defs.md#tsvversionoptionsoutputtypedef) 
## ListReadSetActivationJobsRequestPaginateTypeDef

```python
# ListReadSetActivationJobsRequestPaginateTypeDef definition

class ListReadSetActivationJobsRequestPaginateTypeDef(TypedDict):
    sequenceStoreId: str,
    filter: NotRequired[ActivateReadSetFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ActivateReadSetFilterTypeDef](./type_defs.md#activatereadsetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReadSetActivationJobsRequestRequestTypeDef

```python
# ListReadSetActivationJobsRequestRequestTypeDef definition

class ListReadSetActivationJobsRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ActivateReadSetFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ActivateReadSetFilterTypeDef](./type_defs.md#activatereadsetfiltertypedef) 
## ListReadSetExportJobsRequestPaginateTypeDef

```python
# ListReadSetExportJobsRequestPaginateTypeDef definition

class ListReadSetExportJobsRequestPaginateTypeDef(TypedDict):
    sequenceStoreId: str,
    filter: NotRequired[ExportReadSetFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExportReadSetFilterTypeDef](./type_defs.md#exportreadsetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReadSetExportJobsRequestRequestTypeDef

```python
# ListReadSetExportJobsRequestRequestTypeDef definition

class ListReadSetExportJobsRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ExportReadSetFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ExportReadSetFilterTypeDef](./type_defs.md#exportreadsetfiltertypedef) 
## ListReadSetImportJobsRequestPaginateTypeDef

```python
# ListReadSetImportJobsRequestPaginateTypeDef definition

class ListReadSetImportJobsRequestPaginateTypeDef(TypedDict):
    sequenceStoreId: str,
    filter: NotRequired[ImportReadSetFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ImportReadSetFilterTypeDef](./type_defs.md#importreadsetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReadSetImportJobsRequestRequestTypeDef

```python
# ListReadSetImportJobsRequestRequestTypeDef definition

class ListReadSetImportJobsRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ImportReadSetFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ImportReadSetFilterTypeDef](./type_defs.md#importreadsetfiltertypedef) 
## ListReferenceImportJobsRequestPaginateTypeDef

```python
# ListReferenceImportJobsRequestPaginateTypeDef definition

class ListReferenceImportJobsRequestPaginateTypeDef(TypedDict):
    referenceStoreId: str,
    filter: NotRequired[ImportReferenceFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ImportReferenceFilterTypeDef](./type_defs.md#importreferencefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReferenceImportJobsRequestRequestTypeDef

```python
# ListReferenceImportJobsRequestRequestTypeDef definition

class ListReferenceImportJobsRequestRequestTypeDef(TypedDict):
    referenceStoreId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ImportReferenceFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ImportReferenceFilterTypeDef](./type_defs.md#importreferencefiltertypedef) 
## ListReadSetsRequestPaginateTypeDef

```python
# ListReadSetsRequestPaginateTypeDef definition

class ListReadSetsRequestPaginateTypeDef(TypedDict):
    sequenceStoreId: str,
    filter: NotRequired[ReadSetFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ReadSetFilterTypeDef](./type_defs.md#readsetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReadSetsRequestRequestTypeDef

```python
# ListReadSetsRequestRequestTypeDef definition

class ListReadSetsRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ReadSetFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ReadSetFilterTypeDef](./type_defs.md#readsetfiltertypedef) 
## ListReadSetUploadPartsRequestPaginateTypeDef

```python
# ListReadSetUploadPartsRequestPaginateTypeDef definition

class ListReadSetUploadPartsRequestPaginateTypeDef(TypedDict):
    sequenceStoreId: str,
    uploadId: str,
    partSource: ReadSetPartSourceType,  # (1)
    filter: NotRequired[ReadSetUploadPartListFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ReadSetPartSourceType](./literals.md#readsetpartsourcetype) 
2. See [:material-code-braces: ReadSetUploadPartListFilterTypeDef](./type_defs.md#readsetuploadpartlistfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReadSetUploadPartsRequestRequestTypeDef

```python
# ListReadSetUploadPartsRequestRequestTypeDef definition

class ListReadSetUploadPartsRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    uploadId: str,
    partSource: ReadSetPartSourceType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ReadSetUploadPartListFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: ReadSetPartSourceType](./literals.md#readsetpartsourcetype) 
2. See [:material-code-braces: ReadSetUploadPartListFilterTypeDef](./type_defs.md#readsetuploadpartlistfiltertypedef) 
## ListReferencesRequestPaginateTypeDef

```python
# ListReferencesRequestPaginateTypeDef definition

class ListReferencesRequestPaginateTypeDef(TypedDict):
    referenceStoreId: str,
    filter: NotRequired[ReferenceFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ReferenceFilterTypeDef](./type_defs.md#referencefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReferencesRequestRequestTypeDef

```python
# ListReferencesRequestRequestTypeDef definition

class ListReferencesRequestRequestTypeDef(TypedDict):
    referenceStoreId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ReferenceFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ReferenceFilterTypeDef](./type_defs.md#referencefiltertypedef) 
## ListReferenceStoresRequestPaginateTypeDef

```python
# ListReferenceStoresRequestPaginateTypeDef definition

class ListReferenceStoresRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[ReferenceStoreFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ReferenceStoreFilterTypeDef](./type_defs.md#referencestorefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReferenceStoresRequestRequestTypeDef

```python
# ListReferenceStoresRequestRequestTypeDef definition

class ListReferenceStoresRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[ReferenceStoreFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ReferenceStoreFilterTypeDef](./type_defs.md#referencestorefiltertypedef) 
## ListSequenceStoresRequestPaginateTypeDef

```python
# ListSequenceStoresRequestPaginateTypeDef definition

class ListSequenceStoresRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[SequenceStoreFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SequenceStoreFilterTypeDef](./type_defs.md#sequencestorefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSequenceStoresRequestRequestTypeDef

```python
# ListSequenceStoresRequestRequestTypeDef definition

class ListSequenceStoresRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filter: NotRequired[SequenceStoreFilterTypeDef],  # (1)
```

1. See [:material-code-braces: SequenceStoreFilterTypeDef](./type_defs.md#sequencestorefiltertypedef) 
## ListAnnotationStoresResponseTypeDef

```python
# ListAnnotationStoresResponseTypeDef definition

class ListAnnotationStoresResponseTypeDef(TypedDict):
    annotationStores: List[AnnotationStoreItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnnotationStoreItemTypeDef](./type_defs.md#annotationstoreitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReferenceStoresResponseTypeDef

```python
# ListReferenceStoresResponseTypeDef definition

class ListReferenceStoresResponseTypeDef(TypedDict):
    referenceStores: List[ReferenceStoreDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReferenceStoreDetailTypeDef](./type_defs.md#referencestoredetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSequenceStoresResponseTypeDef

```python
# ListSequenceStoresResponseTypeDef definition

class ListSequenceStoresResponseTypeDef(TypedDict):
    sequenceStores: List[SequenceStoreDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SequenceStoreDetailTypeDef](./type_defs.md#sequencestoredetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVariantStoresResponseTypeDef

```python
# ListVariantStoresResponseTypeDef definition

class ListVariantStoresResponseTypeDef(TypedDict):
    variantStores: List[VariantStoreItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VariantStoreItemTypeDef](./type_defs.md#variantstoreitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReadSetFilesTypeDef

```python
# ReadSetFilesTypeDef definition

class ReadSetFilesTypeDef(TypedDict):
    source1: NotRequired[FileInformationTypeDef],  # (1)
    source2: NotRequired[FileInformationTypeDef],  # (1)
    index: NotRequired[FileInformationTypeDef],  # (1)
```

1. See [:material-code-braces: FileInformationTypeDef](./type_defs.md#fileinformationtypedef) 
2. See [:material-code-braces: FileInformationTypeDef](./type_defs.md#fileinformationtypedef) 
3. See [:material-code-braces: FileInformationTypeDef](./type_defs.md#fileinformationtypedef) 
## ReferenceFilesTypeDef

```python
# ReferenceFilesTypeDef definition

class ReferenceFilesTypeDef(TypedDict):
    source: NotRequired[FileInformationTypeDef],  # (1)
    index: NotRequired[FileInformationTypeDef],  # (1)
```

1. See [:material-code-braces: FileInformationTypeDef](./type_defs.md#fileinformationtypedef) 
2. See [:material-code-braces: FileInformationTypeDef](./type_defs.md#fileinformationtypedef) 
## ListReadSetsResponseTypeDef

```python
# ListReadSetsResponseTypeDef definition

class ListReadSetsResponseTypeDef(TypedDict):
    readSets: List[ReadSetListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReadSetListItemTypeDef](./type_defs.md#readsetlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReadSetImportJobResponseTypeDef

```python
# GetReadSetImportJobResponseTypeDef definition

class GetReadSetImportJobResponseTypeDef(TypedDict):
    id: str,
    sequenceStoreId: str,
    roleArn: str,
    status: ReadSetImportJobStatusType,  # (1)
    statusMessage: str,
    creationTime: datetime,
    completionTime: datetime,
    sources: List[ImportReadSetSourceItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ReadSetImportJobStatusType](./literals.md#readsetimportjobstatustype) 
2. See [:material-code-braces: ImportReadSetSourceItemTypeDef](./type_defs.md#importreadsetsourceitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReadSetImportJobRequestRequestTypeDef

```python
# StartReadSetImportJobRequestRequestTypeDef definition

class StartReadSetImportJobRequestRequestTypeDef(TypedDict):
    sequenceStoreId: str,
    roleArn: str,
    sources: Sequence[StartReadSetImportJobSourceItemTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: StartReadSetImportJobSourceItemTypeDef](./type_defs.md#startreadsetimportjobsourceitemtypedef) 
## FormatOptionsTypeDef

```python
# FormatOptionsTypeDef definition

class FormatOptionsTypeDef(TypedDict):
    tsvOptions: NotRequired[TsvOptionsTypeDef],  # (1)
    vcfOptions: NotRequired[VcfOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: TsvOptionsTypeDef](./type_defs.md#tsvoptionstypedef) 
2. See [:material-code-braces: VcfOptionsTypeDef](./type_defs.md#vcfoptionstypedef) 
## CreateAnnotationStoreResponseTypeDef

```python
# CreateAnnotationStoreResponseTypeDef definition

class CreateAnnotationStoreResponseTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    storeFormat: StoreFormatType,  # (2)
    storeOptions: StoreOptionsOutputTypeDef,  # (3)
    status: StoreStatusType,  # (4)
    name: str,
    versionName: str,
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreFormatType](./literals.md#storeformattype) 
3. See [:material-code-braces: StoreOptionsOutputTypeDef](./type_defs.md#storeoptionsoutputtypedef) 
4. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnnotationStoreResponseTypeDef

```python
# GetAnnotationStoreResponseTypeDef definition

class GetAnnotationStoreResponseTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    status: StoreStatusType,  # (2)
    storeArn: str,
    name: str,
    description: str,
    sseConfig: SseConfigTypeDef,  # (3)
    creationTime: datetime,
    updateTime: datetime,
    tags: Dict[str, str],
    storeOptions: StoreOptionsOutputTypeDef,  # (4)
    storeFormat: StoreFormatType,  # (5)
    statusMessage: str,
    storeSizeBytes: int,
    numVersions: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
3. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
4. See [:material-code-braces: StoreOptionsOutputTypeDef](./type_defs.md#storeoptionsoutputtypedef) 
5. See [:material-code-brackets: StoreFormatType](./literals.md#storeformattype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnnotationStoreResponseTypeDef

```python
# UpdateAnnotationStoreResponseTypeDef definition

class UpdateAnnotationStoreResponseTypeDef(TypedDict):
    id: str,
    reference: ReferenceItemTypeDef,  # (1)
    status: StoreStatusType,  # (2)
    name: str,
    description: str,
    creationTime: datetime,
    updateTime: datetime,
    storeOptions: StoreOptionsOutputTypeDef,  # (3)
    storeFormat: StoreFormatType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
2. See [:material-code-brackets: StoreStatusType](./literals.md#storestatustype) 
3. See [:material-code-braces: StoreOptionsOutputTypeDef](./type_defs.md#storeoptionsoutputtypedef) 
4. See [:material-code-brackets: StoreFormatType](./literals.md#storeformattype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StoreOptionsTypeDef

```python
# StoreOptionsTypeDef definition

class StoreOptionsTypeDef(TypedDict):
    tsvStoreOptions: NotRequired[TsvStoreOptionsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: TsvStoreOptionsTypeDef](./type_defs.md#tsvstoreoptionstypedef) [:material-code-braces: TsvStoreOptionsOutputTypeDef](./type_defs.md#tsvstoreoptionsoutputtypedef) 
## CreateAnnotationStoreVersionResponseTypeDef

```python
# CreateAnnotationStoreVersionResponseTypeDef definition

class CreateAnnotationStoreVersionResponseTypeDef(TypedDict):
    id: str,
    versionName: str,
    storeId: str,
    versionOptions: VersionOptionsOutputTypeDef,  # (1)
    name: str,
    status: VersionStatusType,  # (2)
    creationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VersionOptionsOutputTypeDef](./type_defs.md#versionoptionsoutputtypedef) 
2. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnnotationStoreVersionResponseTypeDef

```python
# GetAnnotationStoreVersionResponseTypeDef definition

class GetAnnotationStoreVersionResponseTypeDef(TypedDict):
    storeId: str,
    id: str,
    status: VersionStatusType,  # (1)
    versionArn: str,
    name: str,
    versionName: str,
    description: str,
    creationTime: datetime,
    updateTime: datetime,
    tags: Dict[str, str],
    versionOptions: VersionOptionsOutputTypeDef,  # (2)
    statusMessage: str,
    versionSizeBytes: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
2. See [:material-code-braces: VersionOptionsOutputTypeDef](./type_defs.md#versionoptionsoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VersionOptionsTypeDef

```python
# VersionOptionsTypeDef definition

class VersionOptionsTypeDef(TypedDict):
    tsvVersionOptions: NotRequired[TsvVersionOptionsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: TsvVersionOptionsTypeDef](./type_defs.md#tsvversionoptionstypedef) [:material-code-braces: TsvVersionOptionsOutputTypeDef](./type_defs.md#tsvversionoptionsoutputtypedef) 
## GetReadSetMetadataResponseTypeDef

```python
# GetReadSetMetadataResponseTypeDef definition

class GetReadSetMetadataResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    sequenceStoreId: str,
    subjectId: str,
    sampleId: str,
    status: ReadSetStatusType,  # (1)
    name: str,
    description: str,
    fileType: FileTypeType,  # (2)
    creationTime: datetime,
    sequenceInformation: SequenceInformationTypeDef,  # (3)
    referenceArn: str,
    files: ReadSetFilesTypeDef,  # (4)
    statusMessage: str,
    creationType: CreationTypeType,  # (5)
    etag: ETagTypeDef,  # (6)
    creationJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: ReadSetStatusType](./literals.md#readsetstatustype) 
2. See [:material-code-brackets: FileTypeType](./literals.md#filetypetype) 
3. See [:material-code-braces: SequenceInformationTypeDef](./type_defs.md#sequenceinformationtypedef) 
4. See [:material-code-braces: ReadSetFilesTypeDef](./type_defs.md#readsetfilestypedef) 
5. See [:material-code-brackets: CreationTypeType](./literals.md#creationtypetype) 
6. See [:material-code-braces: ETagTypeDef](./type_defs.md#etagtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReferenceMetadataResponseTypeDef

```python
# GetReferenceMetadataResponseTypeDef definition

class GetReferenceMetadataResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    referenceStoreId: str,
    md5: str,
    status: ReferenceStatusType,  # (1)
    name: str,
    description: str,
    creationTime: datetime,
    updateTime: datetime,
    files: ReferenceFilesTypeDef,  # (2)
    creationType: ReferenceCreationTypeType,  # (3)
    creationJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ReferenceStatusType](./literals.md#referencestatustype) 
2. See [:material-code-braces: ReferenceFilesTypeDef](./type_defs.md#referencefilestypedef) 
3. See [:material-code-brackets: ReferenceCreationTypeType](./literals.md#referencecreationtypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnnotationImportResponseTypeDef

```python
# GetAnnotationImportResponseTypeDef definition

class GetAnnotationImportResponseTypeDef(TypedDict):
    id: str,
    destinationName: str,
    versionName: str,
    roleArn: str,
    status: JobStatusType,  # (1)
    statusMessage: str,
    creationTime: datetime,
    updateTime: datetime,
    completionTime: datetime,
    items: List[AnnotationImportItemDetailTypeDef],  # (2)
    runLeftNormalization: bool,
    formatOptions: FormatOptionsTypeDef,  # (3)
    annotationFields: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: AnnotationImportItemDetailTypeDef](./type_defs.md#annotationimportitemdetailtypedef) 
3. See [:material-code-braces: FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAnnotationImportRequestRequestTypeDef

```python
# StartAnnotationImportRequestRequestTypeDef definition

class StartAnnotationImportRequestRequestTypeDef(TypedDict):
    destinationName: str,
    roleArn: str,
    items: Sequence[AnnotationImportItemSourceTypeDef],  # (1)
    versionName: NotRequired[str],
    formatOptions: NotRequired[FormatOptionsTypeDef],  # (2)
    runLeftNormalization: NotRequired[bool],
    annotationFields: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AnnotationImportItemSourceTypeDef](./type_defs.md#annotationimportitemsourcetypedef) 
2. See [:material-code-braces: FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef) 
## CreateAnnotationStoreRequestRequestTypeDef

```python
# CreateAnnotationStoreRequestRequestTypeDef definition

class CreateAnnotationStoreRequestRequestTypeDef(TypedDict):
    storeFormat: StoreFormatType,  # (1)
    reference: NotRequired[ReferenceItemTypeDef],  # (2)
    name: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    versionName: NotRequired[str],
    sseConfig: NotRequired[SseConfigTypeDef],  # (3)
    storeOptions: NotRequired[StoreOptionsTypeDef],  # (4)
```

1. See [:material-code-brackets: StoreFormatType](./literals.md#storeformattype) 
2. See [:material-code-braces: ReferenceItemTypeDef](./type_defs.md#referenceitemtypedef) 
3. See [:material-code-braces: SseConfigTypeDef](./type_defs.md#sseconfigtypedef) 
4. See [:material-code-braces: StoreOptionsTypeDef](./type_defs.md#storeoptionstypedef) 
## CreateAnnotationStoreVersionRequestRequestTypeDef

```python
# CreateAnnotationStoreVersionRequestRequestTypeDef definition

class CreateAnnotationStoreVersionRequestRequestTypeDef(TypedDict):
    name: str,
    versionName: str,
    description: NotRequired[str],
    versionOptions: NotRequired[VersionOptionsTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: VersionOptionsTypeDef](./type_defs.md#versionoptionstypedef) 
